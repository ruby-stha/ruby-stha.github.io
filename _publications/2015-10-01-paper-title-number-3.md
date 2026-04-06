---
title: "ProReGen: Progressive Residual Generation under Attribute Correlations"
collection: publications
permalink: /publication/2026-04-23-p3
excerpt: ' '
date: 2026-04-23
venue: 'The Fourteenth International Conference on Learning Representations'
slidesurl: #''
paperurl: 'https://openreview.net/pdf?id=2LzYaW032Q'
citation: 'Shrestha, R., Gopi, A., Meisenzahl, C., Lekhak, B., & Wang, L. ProReGen: Progressive Residual Generation under Attribute Correlations. In The Fourteenth International Conference on Learning Representations.'
---

**Abstract:**

Attribute correlations in the training data will compromise the ability of a deep generative model (DGM) to synthesize images with under-represented attribute combinations (*i.e.,* minority samples). 
Existing approaches mitigate this by data re-sampling to remove attribute correlations seen by the DGM, 
using a classifier to provide *pseudo-supervision* on generated counterfactual samples, 
or incorporating inductive bias to explicitly decompose the generation into independent sub-mechanisms. 
We present ProReGen, a *progressive residual generation* approach inspired by the classical Robinson's transformation, to partial out from an image attribute $\mathbf{x}_2$ its component $m(\mathbf{x}_1)$ that is predictable by other image attributes $\mathbf{x}_1$, and the residual $\gamma = \mathbf{x}_2 - m(\mathbf{x}_1)$ that is not. 
This simplifies the problem of 
learning a DGM $g(\mathbf{x}_1, \mathbf{x}_2)$ conditioned on correlated inputs, 
to learning $\tilde{g}(\mathbf{x}_1, \gamma)$
conditioned on orthogonal inputs. 
It further allows us to 
progressively learn  $\tilde{g}$ 
by first shifting the burden to abundant majority samples to 
learn $\tilde{g}(\mathbf{x}_1, \gamma = 0)$, and then expanding it with additional layers $g_{\text{res}}$ to 
resolve its difference to $\tilde{g}(\mathbf{x}_1, \gamma)$ using residual attribute $\gamma$ on limited minority samples. 
On three benchmark datasets with curated varying strengths of attribute correlation and one dataset with natural attribute correlation, we demonstrate that 
ProReGen---with input orthogonalization and progressive residual learning---improved the correctness of minority generations compared to existing strategies.