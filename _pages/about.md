---
permalink: /
title: "About Me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
  .ruby-home {
    --home-muted: #607481;
    --home-border: #e5eaed;
    --home-accent: #529caa;
    font-size: 0.90em;
  }

  .ruby-home .home-keywords {
    margin: 0 0 20px;
    color: var(--home-muted);
    font-size: 0.9em;
    font-weight: 600;
  }

  .ruby-home .home-intro {
    margin-bottom: 18px;
  }

  .ruby-home .home-themes {
    margin-bottom: 24px;
    padding-left: 22px;
  }

  .ruby-home .home-themes li {
    margin-bottom: 12px;
  }

  /* Availability notice */

  .ruby-home .home-availability {
    margin: 24px 0 34px;
    padding: 13px 16px;
    border-left: 3px solid #64abba;
    border-radius: 0 4px 4px 0;
    background: #f1f7fa;
    font-size: 0.88em;
    line-height: 1.7;
  }

  .ruby-home .home-availability a {
    display: inline-block;
    margin-left: 8px;
    font-weight: 600;
  }

  /* Section headings */

  .ruby-home .home-section-heading {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: baseline;
    gap: 8px 20px;
    margin-top: 34px;
    padding-bottom: 10px;
    border-bottom: 1px solid var(--home-border);
  }

  .ruby-home .home-section-heading h2 {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 1.3em;
    line-height: 1.4;
  }

  .ruby-home .home-section-heading > a {
    font-size: 0.8em;
    font-weight: 700;
    white-space: nowrap;
  }

  /* Research entries */

  .ruby-home .home-project {
    padding: 26px 0 30px;
  }

  .ruby-home .home-project + .home-project {
    border-top: 1px solid var(--home-border);
  }

  .ruby-home .home-project h3 {
    margin: 0 0 8px;
    font-size: 1.05em;
    line-height: 1.5;
  }

  .ruby-home .home-project h3 a {
    color: inherit;
    text-decoration: none;
  }

  .ruby-home .home-project h3 a:hover {
    color: var(--home-accent);
    text-decoration: underline;
  }

  .ruby-home .home-project-meta {
    margin: 0 0 20px;
    color: var(--home-muted);
    font-size: 0.82em;
    line-height: 1.6;
  }

  .ruby-home .home-project-figure {
    width: 100%;
    max-width: 550px;
    margin: 0 auto 22px;
  }

  .ruby-home .home-project-figure a {
    display: block;
  }

  .ruby-home .home-project-image {
    display: block;
    width: 100%;
    max-width: 100%;
    height: auto;
    margin: 0;
    border: 0;
  }

  .ruby-home .home-project-description {
    margin: 0;
    font-size: 0.94em;
    line-height: 1.75;
  }

  /* Paper, Code, and Poster buttons */

  .ruby-home .home-project-links {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 18px;
    font-size: 0.84em;
  }

  .ruby-home .home-project-links a {
    display: inline-block;
    padding: 7px 17px;
    border: 1px solid #c5e0eb;
    border-radius: 6px;
    background: #eaf5fb;
    color: #285f78;
    font-size: 0.95em;
    font-weight: 600;
    line-height: 1.4;
    text-decoration: none;
    transition:
      background-color 0.15s ease,
      border-color 0.15s ease;
  }

  .ruby-home .home-project-links a:hover {
    background: #d8edf7;
    border-color: #9fcbdc;
    text-decoration: none;
  }

  .ruby-home .home-project-links a:focus-visible {
    outline: 2px solid #285f78;
    outline-offset: 3px;
  }

  /* Industry experience */

  .ruby-home .home-industry {
    padding-top: 20px;
  }

  .ruby-home .home-industry-topline {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: baseline;
    gap: 6px 20px;
    margin-bottom: 6px;
  }

  .ruby-home .home-industry-company {
    flex: 1 1 300px;
    margin: 0;
    font-size: 1em;
    line-height: 1.5;
  }

  .ruby-home .home-industry-dates {
    color: var(--home-muted);
    font-size: 0.82em;
    white-space: nowrap;
  }

  .ruby-home .home-industry-roles {
    margin: 6px 0 12px;
    color: var(--home-muted);
    font-size: 0.85em;
    line-height: 1.6;
  }

  .ruby-home .home-industry-description {
    margin: 0;
    font-size: 0.94em;
    line-height: 1.75;
  }

  /* Latest Updates */

  .ruby-home .home-news-row {
    display: grid;
    grid-template-columns: 90px minmax(0, 1fr);
    gap: 16px;
    padding: 14px 0;
    border-bottom: 1px solid #eef1f3;
    font-size: 0.88em;
    line-height: 1.65;
  }

  .ruby-home .home-news-row:last-child {
    border-bottom: 0;
  }

  .ruby-home .home-news-date {
    color: var(--home-muted);
    white-space: nowrap;
  }

  .ruby-home .home-news-copy {
    min-width: 0;
    overflow-wrap: anywhere;
  }

  .ruby-home .home-news-copy p {
    margin: 0;
  }

  .ruby-home .home-news-copy p + p {
    margin-top: 8px;
  }

  /* Justify longer descriptions on larger screens */

  @media (min-width: 768px) {
    .ruby-home .home-project-description,
    .ruby-home .home-industry-description {
      text-align: left;
      hyphens: none;
    }
  }

  /* Balanced desktop spacing and navigation alignment */

  @media (min-width: 1024px) {
    #main,
    .masthead__inner-wrap {
      box-sizing: border-box;
      width: 100%;
      max-width: 1050px;
      margin-left: auto;
      margin-right: auto;
      padding-left: 32px;
      padding-right: 32px;
    }

    #main {
      display: grid;
      grid-template-columns: 220px minmax(0, 1fr);
      column-gap: 40px;
      align-items: start;
    }

    #main::before,
    #main::after {
      display: none;
    }

    #main > .sidebar {
      position: sticky;
      top: 90px;
      float: none;
      clear: none;
      width: 100%;
      max-width: none;
      height: auto;
      max-height: calc(100vh - 110px);
      margin: 0;
      padding: 0;
      overflow-y: auto;
    }

    #main > .page {
      float: none;
      width: 100%;
      min-width: 0;
      margin: 0;
      padding: 0;
    }

    .masthead .greedy-nav .visible-links {
      display: table;
    }

    .masthead .greedy-nav .visible-links > li:first-child {
      box-sizing: border-box;
      width: 260px;
      min-width: 260px;
      padding: 0;
    }

    .masthead .greedy-nav .visible-links > li:first-child > a {
      margin-left: 0;
      margin-right: 0;
    }

    .masthead .greedy-nav .visible-links > li:nth-child(2) > a {
      margin-left: 0;
    }
  }

  /* Mobile layout */

  @media (max-width: 600px) {
    .ruby-home .home-section-heading {
      margin-top: 28px;
    }

    .ruby-home .home-project {
      padding: 22px 0 26px;
    }

    .ruby-home .home-project-figure {
      margin-bottom: 18px;
    }

    .ruby-home .home-news-row {
      grid-template-columns: 1fr;
      gap: 4px;
    }

    .ruby-home .home-industry-company {
      flex-basis: 100%;
    }
  }
</style>

<div class="ruby-home">

  <p class="home-keywords">
    Generative AI &nbsp;·&nbsp; Causal ML &nbsp;·&nbsp; Trustworthy ML
  </p>

  <p class="home-intro">
    I am a final-year PhD candidate in Computing and Information Sciences
    at Rochester Institute of Technology, advised by
    <a href="https://www.rit.edu/cblwang/linwei-wang">Prof. Linwei Wang</a>
    in the
    <a href="https://www.rit.edu/cblwang/directory">Computational Biomedicine Lab</a>.
    My research focuses on building
    <strong>reliable deep generative models</strong>:
    improving their robustness and controllability.
  </p>

  <p>My current work explores these themes in image generation:</p>

  <ul class="home-themes">
    <li>
      <strong>Robustness to attribute correlations.</strong>
      I study how attribute correlations in training data limit
      generative models’ generalization to underrepresented attribute
      combinations, and develop approaches to address this challenge.
    </li>
    <li>
      <strong>Controllable and counterfactual generation.</strong>
      I develop robust causal generative models that account for
      relationships between attributes, aiming for accurate controllable
      and counterfactual generation even when attributes are strongly related.
    </li>
  </ul>

  <div class="home-availability">
    I am seeking full-time <strong>Applied Scientist</strong> or
    <strong>Research Scientist</strong> roles in machine learning,
    with interests spanning generative AI and trustworthy ML,
    starting summer 2027.
    Please feel free to get in touch at
    <strong>rs9466 [at] rit [dot] edu</strong>.
    <a href="{{ '/cv/' | relative_url }}">View CV &rarr;</a>
  </div>

  <section aria-labelledby="selected-research">

    <div class="home-section-heading">
      <h2 id="selected-research">Selected Recent Research</h2>
      <a href="{{ '/publications/' | relative_url }}">
        View all publications &rarr;
      </a>
    </div>

    <article class="home-project">

      <h3>
        Re-Examining the Impact of Observed Feature Correlations
        on Minority Image Generation
      </h3>

      <p class="home-project-meta">
        <strong>Under review</strong>
      </p>

      <figure class="home-project-figure">
        <a
          href="{{ '/images/minority-generation.png' | relative_url }}"
          target="_blank"
          rel="noopener"
          aria-label="Open the minority image generation overview at full size">
          <img
            class="home-project-image"
            src="{{ '/images/minority-generation.png' | relative_url }}"
            alt="Overview of correlated training data, the systematic evaluation, and factors contributing to minority generation failure."
            loading="lazy">
        </a>
      </figure>

      <p class="home-project-description">
        Can generative models reliably produce attribute combinations
        underrepresented in their training data? Designing a multi-metric
        evaluation framework, we systematically evaluate 13+ generative
        models and mitigation strategies across synthetic, natural,
        and medical datasets under increasing feature correlation.
        With this, we identify root causes of failure: covariate shift,
        limited minority sample diversity, mismatched inductive bias,
        and biased classifier supervision, as well as develop a
        theoretical perspective on observed failures by drawing an
        analogy between minority image generation and potential outcome
        estimation in causal inference.
      </p>

    </article>

    <article class="home-project">

      <h3>
        <a href="https://openreview.net/pdf?id=2LzYaW032Q">
          ProReGen: Progressive Residual Generation
          under Attribute Correlations
        </a>
      </h3>

      <p class="home-project-meta">
        <strong>ICLR 2026</strong> &nbsp;·&nbsp; First author
      </p>

      <figure class="home-project-figure">
        <a
          href="{{ '/images/proregen.png' | relative_url }}"
          target="_blank"
          rel="noopener"
          aria-label="Open the ProReGen method diagram at full size">
          <img
            class="home-project-image"
            src="{{ '/images/proregen.png' | relative_url }}"
            alt="ProReGen method: recasting correlated attribute conditioning through residualization and two-stage learning."
            loading="lazy">
        </a>
      </figure>

      <p class="home-project-description">
        Correlations among attributes in training data can cause
        generative models to fail on requested attribute combinations
        that go against those correlations. Inspired by Robinson’s
        partialling-out transformation from causal inference, ProReGen
        turns correlated attributes into orthogonal ones and learns
        progressively: first from abundant correlation-aligned samples,
        then from limited correlation-conflicting samples, which only
        need to teach the model the residual. As a model-agnostic
        framework, ProReGen applies to VAEs, GANs, and diffusion models,
        improving the correctness of generations for underrepresented
        attribute combinations without degrading those for common ones.
      </p>

      <div class="home-project-links">
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

    </article>

  </section>

  <section aria-labelledby="industry-experience">

    <div class="home-section-heading">
      <h2 id="industry-experience">Industry Experience</h2>
      <a href="{{ '/cv/' | relative_url }}">
        Details in CV &rarr;
      </a>
    </div>

    <div class="home-industry">
      <div class="home-industry-topline">
        <h3 class="home-industry-company">
          Deerwalk Inc. (now a Cedar Gate Technologies Company)
        </h3>
        <span class="home-industry-dates">2015–2021</span>
      </div>

      <p class="home-industry-roles">
        Healthcare Analytics &nbsp;·&nbsp; Software Engineering
        &nbsp;·&nbsp; Team Leadership
      </p>

      <p class="home-industry-description">
        Led projects in US healthcare data analytics, reporting,
        and visualization. Progressed from Software Engineering Intern
        to Software Engineer, Team Lead, and Development Manager.
      </p>
    </div>

  </section>

  {% assign full_news = site.pages | where: "permalink", "/news/" | first %}
  {% assign homepage_updates = full_news.updates | where: "year", 2026 %}

  <section aria-labelledby="latest-updates">

    <div class="home-section-heading">
      <h2 id="latest-updates">Latest Updates</h2>
      <a href="{{ '/news/' | relative_url }}">
        View all news &rarr;
      </a>
    </div>

    {% for item in homepage_updates %}
      <div class="home-news-row">
        <span class="home-news-date">
          {{ item.date | escape }}
        </span>
        <div class="home-news-copy">
          {{ item.text | markdownify }}
        </div>
      </div>
    {% endfor %}

  </section>

</div>