---
title: "Fairness Implications of Machine Unlearning: Bias Risks in Removing NSFW Content from Text-to-Image Models"
collection: publications
category: conferences
permalink: /publication/2024-fairness
date: 2024-10-01
venue: 'NeurIPS 2024 Workshop on Regulatable ML'
paperurl: 'files/fairness implication CR.pdf'
citation: '<strong>Xiwen Wei</strong>, Guihong Li, & Radu Marculescu. (2024). &quot;Fairness Implications of Machine Unlearning: Bias Risks in Removing NSFW Content from Text-to-Image Models.&quot; <i>NeurIPS 2024 Workshop on Regulatable ML</i>.'
---

<!-- ```
@inproceedings{
wei2024fairness,
title={Fairness Implications of Machine Unlearning: Bias Risks in Removing {NSFW} Content from Text-to-Image Models},
author={Xiwen Wei and Guihong Li and Radu Marculescu},
booktitle={NeurIPS 2024 Workshop on Regulatable ML},
year={2024},
url={https://openreview.net/forum?id=JMRvA73SIV}
}
``` -->

The rapid development of large-scale text-to-image generative models has raised significant concerns about their potential misuse in generating harmful, misleading, or inappropriate content. To address these safety issues, various machine unlearning methods have been proposed to efficiently remove not-safe-for-work (NSFW) content without the need for complete model re-training. While these unlearning methods effectively enhance model safety, their impact on model fairness remains largely unexplored. In this paper, we examine the fairness implications of NSFW content removal via machine unlearning and discover that some methods can unintentionally amplify existing biases, increasing them by up to 6x. Our findings reveal that this increased bias arises from the biased synthetic training data used during the unlearning process. To mitigate this bias, we employ Bayesian optimization to identify the optimal training data composition, thus balancing safety and fairness.