---
title: "NAX: Neural Architecture and Memristive Xbar based Accelerator Co-design"
collection: publications
permalink: /publications/nax
excerpt: 'This paper is on Neural Network and IMC accelerator architecture co-design.'
date: 2022-06-20
venue: 'DAC'
paperurl: 'https://dl.acm.org/doi/abs/10.1145/3489517.3530476'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
layout: single
header:
    image: /images/nax_arch.png
    # overlay_filter: 0.2  # Optional: adds a dark overlay for better title visibility
    caption: "NAX Framework Overview"
---

Neural Architecture Search (NAS) has provided the ability to design efficient deep neural network (DNN) catered towards different hardwares like GPUs, CPUs etc. However, integrating NAS with Memristive Crossbar Array (MCA) based In-Memory Computing (IMC) accelerator remains an open problem. The hardware efficiency (energy, latency and area) as well as application accuracy (considering device and circuit non-idealities) of DNNs mapped to such hardware are co-dependent on network parameters such as kernel size, depth etc. and hardware architecture parameters such as crossbar size and the precision of analog-to-digital converters. Co-optimization of both network and hardware parameters presents a challenging search space comprising of different kernel sizes mapped to varying crossbar sizes. To that effect, we propose NAX – an efficient neural architecture search engine that co-designs neural network and IMC based hardware architecture. NAX explores the aforementioned search space to determine kernel and corresponding crossbar sizes for each DNN layer to achieve optimal tradeoffs between hardware efficiency and application accuracy. For CIFAR-10 and Tiny ImageNet, our models achieve 0.9% and 18.57% higher accuracy at 30% and -10.47% lower EDAP (energy-delay-area product), compared to baseline ResNet-20 and ResNet-18 models, respectively.