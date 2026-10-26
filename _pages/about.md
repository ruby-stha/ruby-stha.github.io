---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a final-year PhD candidate in Computing and Information Sciences at Rochester Institute of Technology, advised by [Prof. Linwei Wang](https://www.rit.edu/cblwang/linwei-wang) in the [Computational Biomedicine Lab](https://www.rit.edu/cblwang/directory). My research focuses on building **reliable deep generative models**: improving their robustness and controllability, particularly for cases underrepresented in the training data.

My current work explores these themes in computer vision:

- **Robustness to attribute correlations.** I study how attribute correlations in training data make it difficult for generative models to produce images with underrepresented attribute combinations, and explore approaches to addressing this challenge.
- **Controllable and counterfactual generation.** I develop causal generative models that account for relationships between attributes to improve controllable and counterfactual generation under varying strengths of these relationships.

<div class="availability-note">
  I am seeking full-time <strong>Applied Scientist</strong> or <strong>Research Scientist</strong> roles in machine learning, with interests spanning generative AI and trustworthy ML, starting summer 2027. Please feel free to get in touch at <strong>rs9466 [at] rit [dot] edu</strong>.
</div>


<div class="research-header">
  <h2 id="selected-research">Selected Recent Research</h2>
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
      loading="lazy">
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


<style>
  .industry-entry {
    margin: 20px 0 32px;
  }

  .industry-topline {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: baseline;
    gap: 6px 20px;
  }

  .industry-entry .industry-company {
    margin: 0;
    font-size: 1em;
    line-height: 1.5;
  }

  .industry-dates {
    color: #607481;
    font-size: 0.85em;
    white-space: nowrap;
  }

  .industry-entry .industry-roles {
    margin: 6px 0 12px;
    color: #607481;
    font-size: 0.85em;
    line-height: 1.6;
  }

  .industry-entry .industry-description {
    margin: 0;
    line-height: 1.65;
  }
</style>

<div class="research-header">
  <h2 id="industry-experience">Industry Experience</h2>
  <a
    class="all-publications"
    href="{{ '/cv/' | relative_url }}">
    Details in CV &rarr;
  </a>
</div>

<div class="industry-entry">
  <div class="industry-topline">
    <h3 class="industry-company">
      Deerwalk Inc. / Cedar Gate Technologies
    </h3>
    <span class="industry-dates">2015–2021</span>
  </div>

  <p class="industry-roles">
    Software Engineering &nbsp;·&nbsp; Team Leadership
  </p>

  <p class="industry-description">
    Progressed from Software Engineering Intern to Software Engineer, Team Lead, Senior Software Engineer and Development Manager. Contributed to and led projects in healthcare reporting and data visualization.
  </p>
</div>

<!-- ## Education

<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  PhD in Computing & Information Sciences<br>
<span class="university"> &nbsp; &nbsp; &nbsp; Rochester Institute of Technology</span><br><br>
<img src="https://academicpages.github.io/images/favicon.ico" alt="Alt text" width="20" height="20">  Bachelor in Computer Science & Information Technology, 2017<br>
<span class="university">&nbsp; &nbsp; &nbsp; Tribhuvan University, Nepal</span> -->

{% assign full_news = site.pages | where: "permalink", "/news/" | first %}
{% assign homepage_updates = full_news.updates | where: "year", 2026 %}

<section class="ruby-updates" aria-labelledby="latest-updates">
  <div class="updates-header">
    <h2 id="latest-updates">Latest Updates</h2>
    <a class="updates-all" href="{{ '/news/' | relative_url }}">View all news &rarr;</a>
  </div>
  {% for item in homepage_updates %}
    <div class="update-row">
      <span class="update-date">{{ item.date | escape }}</span>
      <div class="update-copy">{{ item.text | markdownify }}</div>
    </div>
  {% endfor %}
</section>
