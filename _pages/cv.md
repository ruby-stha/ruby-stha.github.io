---
layout: archive
title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

<style>
  .cv-header {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    gap: 12px;
    margin-bottom: 20px;
  }

  .cv-header h1 {
    margin: 0;
  }

  .cv-download {
    display: inline-block;
    padding: 8px 18px;
    border: 1px solid #c5e0eb;
    border-radius: 6px;
    background: #eaf5fb;
    color: #285f78;
    font-size: 0.8em;
    font-weight: 600;
    line-height: 1.4;
    text-decoration: none;
  }

  .cv-download:hover {
    background: #d8edf7;
    text-decoration: none;
  }

  .cv-download:focus-visible {
    outline: 2px solid #285f78;
    outline-offset: 3px;
  }

  #cv-pages {
    width: 100%;
  }

  #cv-pages canvas {
    box-sizing: border-box;
    display: block;
    width: 100%;
    height: auto;
    margin: 0 0 20px;
    border: 1px solid #e5eaed;
    background: white;
  }

  #cv-status {
    color: #607481;
    font-size: 0.9em;
  }
</style>

<div class="cv-header">
  <h1>CV</h1>

  <a
    class="cv-download"
    href="{{ '/files/RubyShrestha_Oct2026.pdf' | relative_url }}"
    download>
    Download CV &darr;
  </a>
</div>

<p id="cv-status" role="status">Loading CV…</p>

<div id="cv-pages" aria-label="CV page previews"></div>

<noscript>
  <p>
    Please
    <a href="{{ '/files/RubyShrestha_Oct2026.pdf' | relative_url }}">
      open the PDF
    </a>
    to view my CV.
  </p>
</noscript>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js"></script>

<script>
  (async function () {
    const container = document.getElementById("cv-pages");
    const status = document.getElementById("cv-status");

    try {
      pdfjsLib.GlobalWorkerOptions.workerSrc =
        "https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.worker.min.js";

      const pdf = await pdfjsLib.getDocument({
        url: {{ '/files/RubyShrestha_Oct2026.pdf' | relative_url | jsonify }}
      }).promise;

      for (let number = 1; number <= pdf.numPages; number++) {
        const page = await pdf.getPage(number);
        const original = page.getViewport({ scale: 1 });

        const displayWidth = container.clientWidth || 750;
        const pixelRatio = Math.min(
          window.devicePixelRatio || 1,
          2
        );

        const scale =
          (displayWidth / original.width) * pixelRatio;

        const viewport = page.getViewport({ scale });

        const canvas = document.createElement("canvas");
        canvas.width = Math.ceil(viewport.width);
        canvas.height = Math.ceil(viewport.height);

        canvas.setAttribute("role", "img");
        canvas.setAttribute(
          "aria-label",
          "CV page " + number + " of " + pdf.numPages +
          ". Download the PDF for accessible text."
        );

        container.appendChild(canvas);

        await page.render({
          canvasContext: canvas.getContext("2d"),
          viewport: viewport
        }).promise;
      }

      status.hidden = true;
    } catch (error) {
      status.textContent =
        "The preview could not load. Please use the Download CV link above.";
    }
  })();
</script>