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

<div class="availability-note">
  I am seeking full-time <strong>Applied Scientist or Research Scientist</strong> roles in generative AI, with availability starting <strong>2027</strong>.
  Please feel free to <a href="mailto:rs9466@rit.edu">get in touch</a>.
</div>


<div class="research-header">
  <h2 id="selected-research">Selected Research</h2>
  <a
    class="all-publications"
    href="{{ '/publications/' | relative_url }}">
    View all publications &rarr;
  </a>
</div>

<div class="research-project">

  <h3>
    <a href="https://openreview.net/pdf?id=2LzYaW032Q">
      ProReGen: Progressive Residual Generation under Attribute Correlations
    </a>
  </h3>

  <p class="research-authors">
    <strong>Ruby Shrestha</strong>, Ajay Gopi, Casey Meisenzahl,
    Bipin Lekhak, Linwei Wang<br>
    <strong>ICLR 2026</strong>
  </p>

  <a href="https://openreview.net/pdf?id=2LzYaW032Q">
    <img
      class="research-image"
      src="{{ '/images/proregen.png' | relative_url }}"
      alt="ProReGen method: recasting correlated attribute conditioning through residualization and two-stage learning."
      loading="lazy"
      style="width: 70%; height: auto; margin: 20px auto 24px;">
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

  <div class="research-actions">
    <a href="https://openreview.net/pdf?id=2LzYaW032Q">
      Paper
    </a>
    <a href="https://github.com/ruby-stha/ProReGen_ICLR2026">
      Code
    </a>
    <a href="https://iclr.cc/media/PosterPDFs/ICLR%202026/10011751.png?t=1775575313.3895278">
      Poster
    </a>
  </div>

</div>

## Education

<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  PhD in Computing & Information Sciences<br>
<span class="university" style="font-size:.8em"> &nbsp; &nbsp; &nbsp; Rochester Institute of Technology</span><br><br>
<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  Bachelor in Computer Science & Information Technology, 2017<br>
<span class="university" style="font-size:.8em">&nbsp; &nbsp; &nbsp; Tribhuvan University, Nepal</span>