---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a fifth-year PhD student in Computing and Information Sciences at Rochester Institute of Technology, advised by [Prof. Linwei Wang](https://pht180.rit.edu/cblwang/linwei-wang/) in the [Computational Biomedicine Lab](https://pht180.rit.edu/cblwang/).

My research focuses on deep generative modeling, with an emphasis on controllable generation and robustness. I am broadly interested in developing reliable generative models that move the field of trustworthy AI forward.

My current work explores these themes in computer vision, investigating how correlations among attributes in training data affect image generation, and developing causal generative models for controllable and counterfactual image generation.

<div style="
  background-color: #f3f7fa;
  border-left: 3px solid #52adc8;
  padding: 12px 16px;
  margin: 24px 0;
  border-radius: 4px;
  font-size: 0.9em;
  line-height: 1.6;
  color: #333;
">
  I am seeking full-time <strong>Applied Scientist or Research Scientist roles in generative AI, with availability
  starting <strong>2027</strong>. Please feel free to <a href="mailto:rs9466@rit.edu">get in touch</a>.
</div>

## Selected Research

<div style="
  display: flex;
  flex-wrap: wrap;
  gap: 24px;
  align-items: flex-start;
  margin: 20px 0 30px;
">

  <figure style="flex: 0 1 280px; margin: 0;">
    <img
      src="{{ '/images/proregen_results.png' | relative_url }}"
      alt="Requested digit and color combinations, with generated examples from a baseline diffusion model and ProReGen."
      loading="lazy"
      style="
        display: block;
        width: 100%;
        height: auto;
        border: 1px solid #e5e7eb;
        border-radius: 6px;
      ">
    <figcaption style="
      font-size: 0.8em;
      line-height: 1.5;
      margin-top: 8px;
      color: #555;
    ">
      Generating rare attribute combinations:
      baseline versus ProReGen.
    </figcaption>
  </figure>

  <div style="flex: 1 1 300px; min-width: 0;">
    <h3 style="margin: 0 0 10px;">
      <a href="https://openreview.net/pdf?id=2LzYaW032Q">
        ProReGen: Progressive Residual Generation under Attribute Correlations
      </a>
    </h3>

    <p style="font-size: 0.85em; line-height: 1.6; margin: 0 0 12px;">
      <strong>Ruby Shrestha</strong>, Ajay Gopi, Casey Meisenzahl,
      Bipin Lekhak, Linwei Wang<br>
      <strong>ICLR 2026</strong>
    </p>

    <p style="font-size: 0.9em; line-height: 1.6;">
      Generative models can struggle to produce requested attribute
      combinations when those combinations are rare in training data.
      ProReGen learns from abundant combinations, then uses progressive
      residual learning to capture underrepresented combinations.
      The framework improves attribute correctness across VAEs, GANs,
      and diffusion models.
    </p>

    <p style="font-size: 0.85em; margin-bottom: 0;">
      <a href="https://openreview.net/pdf?id=2LzYaW032Q">Paper</a>
      &nbsp;·&nbsp;
      <a href="https://github.com/ruby-stha/ProReGen_ICLR2026">Code</a>
      &nbsp;·&nbsp;
      <a href="https://iclr.cc/media/PosterPDFs/ICLR%202026/10011751.png?t=1775575313.3895278">Poster</a>
    </p>
  </div>

</div>

[View all publications](/publications/)

**Education**

<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  PhD in Computing & Information Sciences<br>
<span class="university" style="font-size:.8em"> &nbsp; &nbsp; &nbsp; Rochester Institute of Technology</span><br><br>
<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  Bachelor in Computer Science & Information Technology, 2017<br>
<span class="university" style="font-size:.8em">&nbsp; &nbsp; &nbsp; Tribhuvan University, Nepal</span>
