<!-- ---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->

---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
  .publications-page { line-height: 1.65; }
  .publications-page .pub-intro { margin: 0 0 28px; }
  .publications-page .pub-section-title {
    margin: 32px 0 18px;
    padding-bottom: 10px;
    border-bottom: 1px solid #e3e9ed;
  }
  .publications-page .pub-card {
    margin-bottom: 20px;
    padding: 22px 24px;
    border: 1px solid #e2e8ed;
    border-radius: 10px;
    background: #fff;
  }
  .publications-page .pub-meta {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 8px;
    margin-bottom: 12px;
    font-size: 0.8em;
    color: #526570;
  }
  .publications-page .pub-badge {
    padding: 3px 10px;
    border-radius: 5px;
    background: #edf5f9;
    color: #28627a;
    font-weight: 600;
  }
  .publications-page .pub-title {
    margin: 0 0 10px;
    font-size: 1.05em;
    line-height: 1.45;
    overflow-wrap: anywhere;
  }
  .publications-page .pub-title a {
    color: inherit;
    text-decoration: none;
  }
  .publications-page .pub-title a:hover {
    color: #28627a;
    text-decoration: underline;
  }
  .publications-page .pub-authors { margin: 0 0 14px; }
  .publications-page .pub-actions {
    display: flex;
    flex-wrap: wrap;
    align-items: flex-start;
    gap: 8px;
  }
  .publications-page .pub-link,
  .publications-page .pub-link:visited,
  .publications-page .pub-citation > summary {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    box-sizing: border-box;
    min-height: 44px;
    padding: 7px 15px;
    border: 1px solid #d5e6ee;
    border-radius: 6px;
    background: #f3f7fa;
    color: #28627a;
    font: inherit;
    font-size: 0.85em;
    font-weight: 600;
    line-height: 1.4;
    text-decoration: none;
    cursor: pointer;
  }
  .publications-page .pub-citation { margin: 0; min-width: 0; }
  .publications-page .pub-citation > summary { list-style: none; }
  .publications-page .pub-citation > summary::-webkit-details-marker {
    display: none;
  }
  .publications-page .pub-citation > summary::after {
    content: "+";
    margin-left: 8px;
  }
  .publications-page .pub-citation[open] { flex-basis: 100%; }
  .publications-page .pub-citation[open] > summary::after { content: "−"; }
  .publications-page .pub-link:hover,
  .publications-page .pub-citation > summary:hover {
    background: #e4f0f6;
    border-color: #8bbace;
    text-decoration: none;
  }
  .publications-page a:focus-visible,
  .publications-page summary:focus-visible {
    outline: 2px solid #28627a;
    outline-offset: 3px;
  }
  .publications-page .pub-citation-text {
    margin-top: 12px;
    padding: 14px 16px;
    border: 1px solid #e2e8ed;
    border-radius: 6px;
    background: #f8fafb;
    font-size: 0.9em;
    overflow-wrap: anywhere;
  }
  .publications-page .pub-citation-text p { margin: 0; }
  @media (max-width: 600px) {
    .publications-page .pub-card { padding: 18px 16px; }
  }
</style>

<div class="publications-page">
  <p class="pub-intro">
    My publications and manuscripts are also listed on
    <a href="https://scholar.google.com/citations?user=JcG1vjIAAAAJ&amp;hl=en">Google Scholar</a>.
    Click <strong>Citation</strong> to expand a formatted reference.
  </p>

  <h2 class="pub-section-title">Peer-reviewed Publications</h2>

  <article class="pub-card" aria-labelledby="pub-proregen">
    <div class="pub-meta">
      <span class="pub-badge">ICLR</span>
      <span>2026</span>
    </div>
    <h3 class="pub-title" id="pub-proregen">
      <a href="https://openreview.net/forum?id=2LzYaW032Q">ProReGen: Progressive Residual Generation under Attribute Correlations</a>
    </h3>
    <p class="pub-authors"><strong>Ruby Shrestha</strong>, Ajay Gopi, Casey Meisenzahl, Bipin Lekhak, Linwei Wang</p>
    <div class="pub-actions">
      <a class="pub-link" href="https://openreview.net/pdf?id=2LzYaW032Q">Paper</a>
      <a class="pub-link" href="https://github.com/ruby-stha/ProReGen_ICLR2026">Code</a>
      <a class="pub-link" href="https://iclr.cc/media/PosterPDFs/ICLR%202026/10011751.png?t=1775575313.3895278">Poster</a>
      <details class="pub-citation">
        <summary aria-label="Citation for ProReGen">Citation</summary>
        <div class="pub-citation-text">
          <p>Shrestha, R., Gopi, A., Meisenzahl, C., Lekhak, B., &amp; Wang, L. (2026). ProReGen: Progressive Residual Generation under Attribute Correlations. <em>International Conference on Learning Representations (ICLR).</em> https://openreview.net/forum?id=2LzYaW032Q</p>
        </div>
      </details>
    </div>
  </article>

  <article class="pub-card" aria-labelledby="pub-dats">
    <div class="pub-meta">
      <span class="pub-badge">ICLR</span>
      <span>2024</span>
    </div>
    <h3 class="pub-title" id="pub-dats">
      <a href="https://openreview.net/forum?id=EvyYFSxdgB">DATS: Difficulty-Aware Task Sampler for Meta-Learning Physics-Informed Neural Networks</a>
    </h3>
    <p class="pub-authors">Maryam Toloubidokhti, Yubo Ye, Ryan Missel, Xiajun Jiang, Nilesh Kumar, <strong>Ruby Shrestha</strong>, Linwei Wang</p>
    <div class="pub-actions">
      <a class="pub-link" href="https://openreview.net/pdf?id=EvyYFSxdgB">Paper</a>
      <a class="pub-link" href="https://github.com/maryamTolou/DATS_ICLR2024">Code</a>
      <details class="pub-citation">
        <summary aria-label="Citation for DATS">Citation</summary>
        <div class="pub-citation-text">
          <p>Toloubidokhti, M., Ye, Y., Missel, R., Jiang, X., Kumar, N., Shrestha, R., &amp; Wang, L. (2024). DATS: Difficulty-Aware Task Sampler for Meta-Learning Physics-Informed Neural Networks. <em>International Conference on Learning Representations (ICLR).</em> https://openreview.net/forum?id=EvyYFSxdgB</p>
        </div>
      </details>
    </div>
  </article>

  <article class="pub-card" aria-labelledby="pub-dro">
    <div class="pub-meta">
      <span class="pub-badge">FAIMI @ MICCAI</span>
      <span>2023</span>
    </div>
    <h3 class="pub-title" id="pub-dro">
      <a href="https://arxiv.org/abs/2308.06434">Distributionally Robust Optimization and Invariant Representation Learning for Addressing Subgroup Underrepresentation: Mechanisms and Limitations</a>
    </h3>
    <p class="pub-authors" style="margin-bottom: 4px;">
      Nilesh Kumar<sup>*</sup>,
      <strong>Ruby Shrestha</strong><sup>*</sup>,
      Zhiyuan Li, Linwei Wang
    </p>
    <p style="font-size: 0.8em; color: #607481; margin: 0 0 14px;">
      <sup>*</sup> Equal contribution.
    </p>
    <div class="pub-actions">
      <a class="pub-link" href="https://arxiv.org/pdf/2308.06434">Paper</a>
      <details class="pub-citation">
        <summary aria-label="Citation for subgroup underrepresentation paper">Citation</summary>
        <div class="pub-citation-text">
          <p>Kumar, N., Shrestha, R., Li, Z., &amp; Wang, L. (2023). Distributionally Robust Optimization and Invariant Representation Learning for Addressing Subgroup Underrepresentation: Mechanisms and Limitations. In <em>Clinical Image-Based Procedures, Fairness of AI in Medical Imaging, and Ethical and Philosophical Issues in Medical Imaging</em> (pp. 183–193). Springer. https://arxiv.org/abs/2308.06434</p>
        </div>
      </details>
    </div>
  </article>

  <h2 class="pub-section-title">Preprints</h2>

  <article class="pub-card" aria-labelledby="pub-pulsar">
    <div class="pub-meta">
      <span class="pub-badge">arXiv preprint</span>
      <span>2026</span>
    </div>
    <h3 class="pub-title" id="pub-pulsar">
      <a href="https://arxiv.org/abs/2609.03056">Single-pulse reanalysis of the 2024 Vela glitch and new observations of PSR J0437−4715 and PSR J1644−4559</a>
    </h3>
    <p class="pub-authors">Carlos O. Lousto, <strong>Ruby Shrestha</strong>, Ezequiel Zubieta, Susana B. Araujo Furlan, Guillermo Gancio, Federico García, Santiago del Palacio, Ryan Missel, Linwei Wang</p>
    <div class="pub-actions">
      <a class="pub-link" href="https://arxiv.org/pdf/2609.03056">Paper</a>
      <details class="pub-citation">
        <summary aria-label="Citation for Vela glitch paper">Citation</summary>
        <div class="pub-citation-text">
          <p>Lousto, C. O., Shrestha, R., Zubieta, E., Araujo Furlan, S. B., Gancio, G., García, F., del Palacio, S., Missel, R., &amp; Wang, L. (2026). <em>Single-pulse reanalysis of the 2024 Vela glitch and new observations of PSR J0437−4715 and PSR J1644−4559.</em> arXiv:2609.03056. https://arxiv.org/abs/2609.03056</p>
        </div>
      </details>
    </div>
  </article>
</div>
