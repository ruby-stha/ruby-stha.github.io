---
title: "Distributionally Robust Optimization and Invariant Representation Learning for Addressing Subgroup Underrepresentation: Mechanisms and Limitations"
collection: publications
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: ' '
date: 2023-08-12
venue: 'Fairness of AI in Medical Imaging (FAIMI @ MICCAI)'
slidesurl: #'http://ruby-stha.github.io/files/paper1.pdf'
paperurl: 'https://arxiv.org/pdf/2308.06434'
citation: 'Kumar, N., Shrestha, R., Li, Z., & Wang, L. (2023, October). Distributionally Robust Optimization and Invariant Representation Learning for Addressing Subgroup Underrepresentation: Mechanisms and Limitations. In Workshop on Clinical Image-Based Procedures (pp. 183-193). Cham: Springer Nature Switzerland.'
---

**Abstract:**

Spurious correlation caused by subgroup underrepresentation has received increasing attention as a source of bias that can be perpetuated by deep neural networks (DNNs). Distributionally robust optimization has shown success in addressing this bias, although the underlying working mechanism mostly relies on upweighting under-performing samples as surrogates for those underrepresented in data. At the same time, while invariant representation learning has been a powerful choice for removing nuisance-sensitive features, it has been little considered in settings where spurious correlations are caused by significant underrepresentation of subgroups. In this paper, we take the first step to better understand and improve the mechanisms for debiasing spurious correlation due to subgroup underrepresentation in medical image classification. Through a comprehensive evaluation study, we first show that 1) generalized reweighting of under-performing samples can be problematic when bias is not the only cause for poor performance, while 2) naive invariant representation learning suffers from spurious correlations itself. We then present a novel approach that leverages robust optimization to facilitate the learning of invariant representations at the presence of spurious correlations. Finetuned classifiers utilizing such representation demonstrated improved abilities to reduce subgroup performance disparity, while maintaining high average and worst-group performance.

