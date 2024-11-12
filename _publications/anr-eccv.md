---
title: "Attention Beats Linear for Fast Implicit Neural Representation Generation"
collection: publications
category: conferences
permalink: /publication/anr-eccv
excerpt: 'This paper is about fixing template issue #693.'
date: 2024-10-01
venue: 'ECCV2024'
paperurl: 'https://arxiv.org/pdf/2407.15355'
citation: 'Zhang, S., Liu, K., Gu, J., Cai, X., Wang, Z., Bu, J., & Wang, H. (2024). Attention beats linear for fast implicit neural representation generation. arXiv preprint arXiv:2407.15355.'
---

Implicit Neural Representation (INR) has gained increasing popularity as a data representation method, serving as a prerequisite for innovative generation models. Unlike gradient-based methods, which exhibit lower efficiency in inference, the adoption of hyper-network for generating parameters in Multi-Layer Perceptrons (MLP), responsible for executing INR functions, has surfaced as a promising and efficient alternative. However, as a global continuous function, MLP is challenging in modeling highly discontinuous signals, resulting in slow convergence during the training phase and inaccurate reconstruction performance. Moreover, MLP requires massive representation parameters, which implies inefficiencies in data representation. In this paper, we propose a novel Attention-based Localized INR (ANR) composed of a localized attention layer (LAL) and a global MLP that integrates coordinate features with data features and converts them to meaningful outputs. Subsequently, we design an instance representation framework that delivers a transformer-like hyper-network to represent data instances as a compact representation vector. With instance-specific representation vector and instance-agnostic ANR parameters, the target signals are well reconstructed as a continuous function. We further address aliasing artifacts with variational coordinates when obtaining the super-resolution inference results. Extensive experimentation across four datasets showcases the notable efficacy of our ANR method, e.g. enhancing the PSNR value from 37.95dB to 47.25dB on the CelebA dataset. 