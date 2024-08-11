---
title: "DATS: Difficulty-Aware Task Sampler for Meta-Learning Physics-Informed Neural Networks"
collection: publications
permalink: /publication/2010-10-01-paper-title-number-2
excerpt: ' '
date: 2024-01-01
venue: 'The Twelfth International Conference on Learning Representations'
slidesurl: #''
paperurl: 'https://openreview.net/pdf?id=EvyYFSxdgB'
citation: 'Toloubidokhti, M., Ye, Y., Missel, R., Jiang, X., Kumar, N., Shrestha, R., & Wang, L. DATS: Difficulty-Aware Task Sampler for Meta-Learning Physics-Informed Neural Networks. In The Twelfth International Conference on Learning Representations.'
---

**Abstract:**

Advancements in deep learning have led to the development of physics-informed neural networks (PINNs) for solving partial differential equations (PDEs) without being supervised by PDE solutions. While vanilla PINNs require training one network per PDE configuration, recent works have showed the potential to metalearn PINNs across a range of PDE configurations. It is however known that PINN training is associated with different levels of difficulty, depending on the underlying PDE configurations or the number of residual sampling points available. Existing meta-learning approaches, however, treat all PINN tasks equally. We address this gap by introducing a novel difficulty-aware task sampler (DATS) for meta-learning of PINNs. We derive an optimal analytical solution to optimize the probability for sampling individual PINN tasks in order to minimize their validation loss across tasks. We further present two alternative strategies to utilize this sampling probability to either adaptively weigh PINN tasks, or dynamically allocate optimal residual points across tasks. We evaluated DATS against uniform and self-paced task-sampling baselines on two representative meta-PINN models, across five benchmark PDEs as well as three different residual point sampling strategies. The results demonstrated that DATS was able to improve the accuracy of meta-learned PINN solutions when reducing performance disparity across PDE configurations, at only a fraction of residual sampling budgets required by its baselines.