---
title: "Algorithm Hardware Co-design for ADC-Less Compute In-Memory Accelerator"
collection: publications
permalink: /publication/hcim_extension
excerpt: 'This paper is an extension of HCiM showing accuracy considering the analog non-idealities in the crossbar array.'
date: 2024-11-20
venue: 'TCASAI'
paperurl: 'https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10750360'
# citation: 'Your Name, You. (2010). &quot;Paper Title Number 2.&quot; <i>Journal 1</i>. 1(2).'
---

The increasing pervasiveness of artificial intelligence (AI), particularly deep learning demands high-performing yet efficient hardware resources at the edge. Analog compute-inmemory (CiM) architectures have tremendous potential to accelerate AI at the edge by reducing data movement between memory and compute units and exploiting parallelism. However, to fully reap the benefits of analog CiM, it is imperative to deal with the area, latency, and power overheads introduced by high-precision analog-to-digital converters (ADCs). In this work, we propose a hardware-algorithm co-design approach to reduce ADC overhead in analog CiM architectures. We designed a deep neural network (DNN) quantization framework tailored to analog CiM hardware architectures, integrating essential features such as tiling, bit-slicing, and layer mapping. Moreover, we also developed an ADC-Less hybrid analog-digital CiM hardware architecture HCiM that can efficiently process the DNNs trained using our framework. Additionally, we studied the effects of nonidealities in analog CiM on DNN accuracy. Using our hardwareaware training methodology, we can perform extremely low precision quantization and reduce the required ADC precision to binary (1-bit) or ternary (1.5-bit). Compared to an analog CiM baseline architecture using 7 and 4-bit ADC, HCiM achieves energy reductions up to 28× and 12×, respectively. Furthermore, in the presence of analog non-idealities, DNN mapped to HCiM exhibits a minimal drop in accuracy.