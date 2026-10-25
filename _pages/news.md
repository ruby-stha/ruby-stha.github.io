---
layout: archive
title: News
permalink: /news/
author_profile: true
updates:
- section: '2026'
  year: 2026
  date: Oct 2026
  text: Served as a reviewer for **ICLR 2027**.
- section: '2026'
  year: 2026
  date: Jul 2026
  text: Served as a reviewer for the journal **Computerized Medical Imaging and Graphics**.
- section: '2026'
  year: 2026
  date: May 2026
  text: Successfully defended my **PhD dissertation proposal**.
- section: '2026'
  year: 2026
  date: Apr 2026
  text: 'Presented a poster on *[ProReGen: Progressive Residual Generation under Attribute Correlations](https://openreview.net/forum?id=2LzYaW032Q)*
    at **ICLR 2026**.'
- section: '2026'
  year: 2026
  date: Feb 2026
  text: Gave a talk on *Heart Seat*, a home health monitoring system developed through a collaboration between [Casana](https://casanacare.com/)
    and the [Computational Biomedicine Lab](https://www.rit.edu/cblwang/directory), at the **Take Heart Go Red** event.
- section: '2026'
  year: 2026
  date: Jan 2026
  text: 'Our paper, [ProReGen: Progressive Residual Generation under Attribute Correlations](https://openreview.net/forum?id=2LzYaW032Q),
    was accepted at **ICLR 2026**.'
- section: '2025'
  year: 2025
  date: Nov 2025
  text: 'Gave a guest lecture on *Robustness of Deep Learning Models to Observed Attribute Correlations: Exploring Impact
    and Potential Solution* in **CISC-865 Deep Learning** course at RIT.'
- section: '2024'
  year: 2024
  date: Oct 2024
  text: Gave a talk on *Spurious Correlations and Bias in AI Systems* at a seminar for clinical and behavioral health health psychology interns at RIT.
- section: '2023'
  year: 2023
  date: Oct 2023
  text: 'Our paper, [Distributionally Robust Optimization and Invariant Representation Learning for Addressing
    Subgroup Underrepresentation: Mechanisms and Limitations](https://arxiv.org/abs/2308.06434), was published at **FAIMI,
    MICCAI 2023**.'
- section: '2023'
  year: 2023
  date: May 2023
  text: Passed my **PhD Research Potential Assessment (RPA)**.
- section: '2023'
  year: 2023
  date: Feb 2023
  text: Received the **Dr. Russell & Melissa Bessette Award for Doctoral Student Excellence** at RIT.
- section: '2022'
  year: 2022
  date: Aug 2022
  text: Started my **PhD in Computing and Information Sciences at RIT**, joining the [Computational Biomedicine Lab](https://www.rit.edu/cblwang/directory)
    under the supervision of Prof. Linwei Wang.
- section: Earlier Highlights
  year: 2019
  date: Sep 2019
  text: Received the **National Female Education Award** from the Government of Nepal.
- section: Earlier Highlights
  year: 2018
  date: Aug 2018
  text: 'Gave an oral presentation on *Maze Solving with Anomaly Tolerant Dead End Filling and A*: Implementation and Analysis*
    at the **Fifth International Conference on Information Technology for Development (IT4D)**.'
- section: Earlier Highlights
  year: 2018
  date: Apr 2018
  text: Graduated with a **Bachelor’s degree in Computer Science and Information Technology** from Tribhuvan University.
- section: Earlier Highlights
  year: 2016
  date: Apr 2016
  text: Won the **International Girls in ICT Day Hackathon**.
---

<style>
  .ruby-updates { margin: 28px 0; }
  .ruby-updates .updates-header { display: flex; flex-wrap: wrap; align-items: baseline; justify-content: space-between; gap: 8px 20px; border-bottom: 1px solid #e3e9ed; padding-bottom: 12px; margin-bottom: 6px; }
  .ruby-updates .updates-header h2 { margin: 0; padding: 0; border: 0; }
  .ruby-updates .updates-all { font-size: 0.8em; white-space: nowrap; text-decoration: none; }
  .ruby-updates .updates-all:hover { text-decoration: underline; }
  .ruby-updates .updates-year { margin: 28px 0 4px; border-bottom: 1px solid #e3e9ed; padding-bottom: 10px; }
  .ruby-updates .update-row { display: grid; grid-template-columns: 110px minmax(0, 1fr); gap: 18px; align-items: start; padding: 15px 0; border-bottom: 1px solid #edf0f2; }
  .ruby-updates .update-date { display: inline-block; padding: 4px 8px; border-radius: 5px; background: #f3f7fa; color: #28627a; font-size: 0.8em; font-weight: 600; text-align: center; line-height: 1.6; }
  .ruby-updates .update-copy { min-width: 0; font-size: 0.95em; line-height: 1.65; overflow-wrap: anywhere; }
  .ruby-updates .update-copy p { margin: 0; }
  .ruby-updates a:focus-visible { outline: 2px solid #28627a; outline-offset: 3px; }
  @media (max-width: 600px) {
    .ruby-updates .update-row { grid-template-columns: minmax(0, 1fr); gap: 8px; }
    .ruby-updates .update-date { justify-self: start; }
  }
</style>

<div class="ruby-updates">
  {% assign news_sections = page.updates | group_by: "section" %}
  {% for group in news_sections %}
    <h2 class="updates-year">{{ group.name | escape }}</h2>
    {% for item in group.items %}
      <div class="update-row">
        <span class="update-date">{{ item.date | escape }}</span>
        <div class="update-copy">{{ item.text | markdownify }}</div>
      </div>
    {% endfor %}
  {% endfor %}
</div>
