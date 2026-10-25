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

<div style="background-color: #f3f7fa; border-left: 3px solid #52adc8; padding: 12px 16px; margin: 24px 0; border-radius: 4px; font-size: 0.9em; line-height: 1.6; color: #333;">
  I am seeking full-time <strong>Applied Scientist or Research Scientist</strong> roles in generative AI, with availability starting <strong>2027</strong>.
  Please feel free to <a href="mailto:rs9466@rit.edu">get in touch</a>.
</div>

## Selected Research

<div style="margin: 20px 0 30px;">
  <h3 style="margin: 0 0 10px;">
    <a href="https://openreview.net/pdf?id=2LzYaW032Q">
      ProReGen: Progressive Residual Generation under Attribute Correlations
    </a>
  </h3>
  <p style="margin: 0 0 12px;">
    <strong>Ruby Shrestha</strong>, Ajay Gopi, Casey Meisenzahl,
    Bipin Lekhak, Linwei Wang<br>
    <strong>ICLR 2026</strong>
  </p>
  <a href="https://openreview.net/pdf?id=2LzYaW032Q">
    <img
      src="{{ '/images/proregen.png' | relative_url }}"
      alt="ProReGen method: recasting correlated attribute conditioning through residualization and two-stage learning."
      loading="lazy"
      style="display: block; width: 75%; height: auto; margin: 16px 0 20px;">
  </a>
  <p>
    Correlations among attributes in training data can cause generative
    models to struggle with requested combinations that conflict with
    those correlations. ProReGen addresses this through attribute
    residualization and progressive learning: it first learns from
    abundant, correlation-aligned samples, then uses limited
    correlation-conflicting samples to learn residual information.
    The framework improves attribute correctness for underrepresented
    combinations across VAEs, GANs, and diffusion models.
  </p>
  <p style="margin-bottom: 0;">
    <a href="https://openreview.net/pdf?id=2LzYaW032Q">Paper</a>
    &nbsp;·&nbsp;
    <a href="https://github.com/ruby-stha/ProReGen_ICLR2026">Code</a>
    &nbsp;·&nbsp;
    <a href="https://iclr.cc/media/PosterPDFs/ICLR%202026/10011751.png?t=1775575313.3895278">Poster</a>
  </p>
</div>

[View all publications]({{ '/publications/' | relative_url }})

**Education**

<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  PhD in Computing & Information Sciences<br>
<span class="university" style="font-size:.8em"> &nbsp; &nbsp; &nbsp; Rochester Institute of Technology</span><br><br>
<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  Bachelor in Computer Science & Information Technology, 2017<br>
<span class="university" style="font-size:.8em">&nbsp; &nbsp; &nbsp; Tribhuvan University, Nepal</span>