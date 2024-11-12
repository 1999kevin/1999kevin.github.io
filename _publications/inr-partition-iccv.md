---
title: "Partition Speeds up Learning Implicit Neural Representations Based on Exponential-Increase Hypothesis"
collection: publications
category: conferences
permalink: /publication/inr-partition-iccv
excerpt: 'This paper is about fixing template issue #693.'
date: 2023-10-01
venue: 'ICCV2023, Paris, France'
paperurl: 'https://openaccess.thecvf.com/content/ICCV2023/papers/Liu_Partition_Speeds_Up_Learning_Implicit_Neural_Representations_Based_on_Exponential-Increase_ICCV_2023_paper.pdf'
#citation: 'Liu, Ke, et al. "Partition speeds up learning implicit neural representations based on exponential-increase hypothesis." Proceedings of the IEEE/CVF International Conference on Computer Vision. 2023.'
Author: 'Ke Liu, Feng Liu, Haishuai Wang, Ning Ma, Jiajun Bu, Bo Han'
---

Implicit neural representations (INRs) aim to learn a continuous function (i.e., a neural network) to represent an image, where the input and output of the function are pixel coordinates and RGB/Gray values, respectively. However, images tend to consist of many objects whose colors are not perfectly consistent, resulting in the challenge that image is actually a discontinuous piecewise function and cannot be well estimated by a continuous function. In this paper, we empirically investigate that if a neural network is enforced to fit a discontinuous piecewise function to reach a fixed small error, the time costs will increase exponentially with respect to the boundaries in the spatial domain of the target signal. We name this phenomenon the exponential-increase hypothesis. Under the exponential-increase hypothesis, learning INRs for images with many objects will converge very slowly. To address this issue, we first prove that partitioning a complex signal into several sub-regions and utilizing piecewise INRs to fit that signal can significantly speed up the convergence. Based on this fact, we introduce a simple partition mechanism to boost the performance of two INR methods for image reconstruction: one for learning INRs, and the other for learning-to-learn INRs. In both cases, we partition an image into different sub-regions and dedicate smaller networks for each part. In addition, we further propose two partition rules based on regular grids and semantic segmentation maps, respectively. Extensive experiments validate the effectiveness of the proposed partitioning methods in terms of learning INR for a single image (ordinary learning framework) and the learning-to-learn framework.