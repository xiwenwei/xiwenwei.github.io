---
title: "Online-LoRA: Task-free Online Continual Learning via Low Rank Adaptation"
collection: publications
category: conferences
permalink: /publication/2024-olora
date: 2025-03-01
venue: 'Proc. IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)'
paperurl: 'files/Online-LoRA_WACV2025_page.pdf'
citation: '<strong>Xiwen Wei</strong>, Guihong Li, & Radu Marculescu. (2025). &quot;Online-LoRA: Task-free Online Continual Learning via Low Rank Adaptation.&quot; <i>Proc. IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)</i>.'
---

<!-- @inproceedings{xiwenwei_wacv,
  author = {Xiwen Wei and Guihong Li and Radu Marculescu},
  title = {Online-Lo{RA}: Task-free Online Continual Learning via Low Rank Adaptation},
  booktitle = {Proc. IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},
  year = {2025},
  pages = {}
} -->

<!-- ```
@inproceedings{
wei2024onlinelora,
title={Online-Lo{RA}: Task-free Online Continual Learning via Low Rank Adaptation},
author={Xiwen Wei and Guihong Li and Radu Marculescu},
booktitle={NeurIPS 2024 Workshop on Scalable Continual Learning for Lifelong Foundation Models},
year={2024},
url={https://openreview.net/forum?id=X7OKRr09OS}
}
``` -->

[![paper](https://img.shields.io/badge/arXiv-Paper-<COLOR>.svg)](https://arxiv.org/abs/2411.05663)

Catastrophic forgetting is a significant challenge in online continual learning (OCL), especially for non-stationary data streams that do not have well-defined task boundaries. This challenge is exacerbated by the memory constraints and privacy concerns inherent in rehearsal buffers. To tackle catastrophic forgetting, in this paper, we introduce Online-LoRA, a novel framework for task-free OCL. Online-LoRA allows to finetune pre-trained Vision Transformer (ViT) models in real-time to address the limitations of rehearsal buffers and leverage pre-trained models’ performance benefits. As the main contribution, our approach features a novel online weight regularization strategy to identify and consolidate important model parameters. Moreover, Online-LoRA leverages the training dynamics of loss values to enable the automatic recognition of the data distribution shifts. Extensive experiments across many task-free OCL scenarios and benchmark datasets (including CIFAR-100, ImageNet-R, ImageNet-S, CUB-200 and CORe50) demonstrate that Online-LoRA can be robustly adapted to various ViT architectures, while achieving better performance compared to SOTA methods. Our code is available [here](https://github.com/Christina200/Online-LoRA-official.git). 