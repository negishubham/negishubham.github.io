---
title: "Best of both worlds: hybrid SNN-ANN architecture for event-based optical flow estimation"
collection: publications
permalink: /publication/bobw
excerpt: 'This paper proposes a hybrid SNN-ANN model to efficiently process the sparse spatio-temporal data from event-based camera '
date: 2024-04-20
venue: 'IROS 2024'
paperurl: 'https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10802844'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

In the field of robotics, event-based cameras are emerging as a promising low-power alternative to traditional frame-based cameras for capturing high-speed motion and high dynamic range scenes. This is due to their sparse and asynchronous event outputs. Spiking Neural Networks (SNNs) with their asynchronous event-driven compute, show great potential for extracting the spatio-temporal features from these event streams. In contrast, the standard Analog Neural Networks (ANNs1) fail to process event data effectively. However, training SNNs is difficult due to additional trainable parameters (thresholds and leaks), vanishing spikes at deeper layers, and a non-differentiable binary activation function. Furthermore, an additional data structure, “membrane potential", responsible for keeping track of temporal information, must be fetched and updated at every timestep in SNNs. To overcome these challenges, we propose a novel SNN-ANN hybrid architecture that combines the strengths of both. Specifically, we leverage the asynchronous compute capabilities of SNN layers to effectively extract the input temporal information. Concurrently, the ANN layers facilitate training and efficient hardware deployment on traditional machine learning hardware such as GPUs. We provide extensive experimental analysis for assigning each layer to be spiking or analog, leading to a network configuration optimized for performance and ease of training. We evaluate our hybrid architecture for optical flow estimation on DSEC-flow and Multi-Vehicle Stereo Event-Camera (MVSEC) datasets. On the DSEC-flow dataset, the hybrid SNN-ANN architecture achieves a 40% reduction in average endpoint error (AEE) with 22% lower energy consumption compared to Full-SNN, and 48% lower AEE compared to Full-ANN, while maintaining comparable energy usage.
