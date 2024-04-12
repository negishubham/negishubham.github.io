---
title: "HCiM: ADC-Less Hybrid Analog-Digital Compute in Memory Accelerator for Deep Learning Workloads"
collection: publications
permalink: /publication/2010-10-01-paper-title-number-2
excerpt: 'This paper proposes an adcless hyrbid analog digital CiM accelerator'
date: 20-04-2024
venue: 'under review'
paperurl: 'https://arxiv.org/abs/2403.13577'
citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

Analog Compute-in-Memory (CiM) accelerators are increasingly recognized for their efficiency in accelerating Deep Neural Networks (DNN). However, their dependence on Analog-to-Digital Converters (ADCs) for accumulating partial sums from crossbars leads to substantial power and area overhead. Moreover, the high area overhead of ADCs constrains the throughput due to the limited number of ADCs that can be integrated per crossbar. An approach to mitigate this issue involves the adoption of extreme low-precision quantization (binary or ternary) for partial sums. Training based on such an approach eliminates the need for ADCs. While this strategy effectively reduces ADC costs, it introduces the challenge of managing numerous floating-point scale factors, which are trainable parameters like DNN weights. These scale factors must be multiplied with the binary or ternary outputs at the columns of the crossbar to ensure system accuracy. To that effect, we propose an algorithm-hardware co-design approach, where DNNs are first trained with quantization-aware training. Subsequently, we introduce HCiM, an ADC-Less Hybrid Analog-Digital CiM accelerator. HCiM uses analog CiM crossbars for performing Matrix-Vector Multiplication operations coupled with a digital CiM array dedicated to processing scale factors. This digital CiM array can execute both addition and subtraction operations within the memory array, thus enhancing processing speed. Additionally, it exploits the inherent sparsity in ternary quantization to achieve further energy savings. Compared to an analog CiM baseline architecture using 7 and 4-bit ADC, HCiM achieves energy reductions up to 28% and 12%, respectively 
