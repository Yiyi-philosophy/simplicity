---
title: ''
image: '2023-03-25-llm-singlegpu/1679629332417.gif'
tags: Explore LLM
---

<!--more-->


# Sourse

## [王燕飞](https://www.zhihu.com/people/nono-nono-66/posts)

[大模型LLMs算法和计算系统重点论文 - AI系统工程师视角Reading List （1） - 王燕飞的文章](https://zhuanlan.zhihu.com/p/608268806)

[大模型LLMs算法和计算系统重点论文 - AI系统工程师视角Reading List （2） - 王燕飞的文章](https://zhuanlan.zhihu.com/p/616200081)

### Flexgen

[Flexgen LLM推理 CPU Offload计算架构到底干了什么事情？ - 王燕飞的文章 - 知乎](https://zhuanlan.zhihu.com/p/615021309)

[Flexgen LLM推理计算环节的量化分析 - 王燕飞的文章 - 知乎](https://zhuanlan.zhihu.com/p/615327112)

[Flexgen LLM推理相关工作 - 怎么思考寻找优化方法 - 王燕飞的文章 - 知乎](https://zhuanlan.zhihu.com/p/615328081)


## Muli

### Methods

[**如何读论文**：](https://www.bilibili.com/video/BV1H44y1t75x/)

[如何判断（你自己的）研究工作的价值[论文精读]](https://www.bilibili.com/video/BV1oL411c7Us/)

[你（被）吐槽过论文不够 novel 吗？[论文精读]](https://www.bilibili.com/video/BV1ea41127Bq/)

### Background Knowledge

[GPT，GPT-2，GPT-3 论文精读[论文精读]] https://www.bilibili.com/video/BV1AF411b7xQ/

[Transformer论文逐段精读[论文精读]] https://www.bilibili.com/video/BV1pu411o7BE/

[Megatron LM 论文精读[论文精读]] https://www.bilibili.com/video/BV1nB4y1R7Yz/

[Zero 论文精读[论文精读]] https://www.bilibili.com/video/BV1tY411g7ZT/

[InstructGPT 论文精读[论文精读·48]] https://www.bilibili.com/video/BV1hd4y187CR/

[Anthropic LLM 论文精读[论文精读·51]] https://www.bilibili.com/video/BV1XY411B7nM/

# **Article**

[How to Read a Paper](https://web.stanford.edu/class/ee384m/Handouts/HowtoReadPaper.pdf)

> 因为LLM应用效果显著（OpenAI chatGPT/GPT-4、meta OPT/LLaMA），所以LLM的计算系统研究工作从专注训练系统设计到推理系统方向拓展，目标降低LLM推理成本、推理门槛，Flexgen提到了几个重要工作，谷歌代表性工作 PaLM inference 、微软代表性工作   Deepspeed-Inference，另外OSDI22年 Orca工作。PaLM inference和Deepspeed-Inference是端到端系统并行系统设计；Orca侧重对变成seq的计算效率提升，设计token level的并行计算系统，侧重系统设计（不单纯是多GPU同构系统上的高性能计算的并行设计，更强调系统化的设计，包含推理计算、调度服务）来提升推理计算的资源利用率。其他还有，FasterTransformer、LightSeq、TurboTransformers 、  Huggingface的Accelerate工作。这类工作比较侧重从计算机系统设计角度研究对LLM推理计算的优化，大部分优化具有无损特性，相对通用性更高（但是部分工作里也存在正交的有损优化，进一步加速系统性能提升）。

**PaLM inference**
[Blog](https://ai.googleblog.com/2022/04/pathways-language-model-palm-scaling-to.html)
![1679629332417](../images/2023-03-25-llm-singlegpu/1679629332417.gif)
[PaLM: Scaling Language Modeling with Pathways](https://arxiv.org/pdf/2204.02311.pdf)

**Deepspeed-Inference**
https://www.deepspeed.ai/inference/
DeepSpeed Inference: Enabling Efficient Inference
of Transformer Models at Unprecedented Scale
https://arxiv.org/pdf/2207.00032.pdf

**Orca**
https://www.usenix.org/conference/osdi22/presentation/yu
https://www.usenix.org/system/files/osdi22-yu.pdf


**FasterTransformer**
[英伟达Fastertransformer源码解读](https://zhuanlan.zhihu.com/p/79528308)
https://github.com/NVIDIA/FasterTransformer


**LightSeq**
https://arxiv.org/abs/2010.13887

**TurboTransformers**
https://arxiv.org/abs/2010.05680


**Huggingface**
https://arxiv.org/abs/1910.03771


> 一类工作是量化（quantization）和稀疏化（sparsification）工作

[Flexgen](https://arxiv.org/pdf/2303.06865.pdf)

[OpenAI 工程师 lilianweng 关于LLM推理计算优化的方法概述](https://lilianweng.github.io/posts/2023-01-10-inference-optimization/)


> Several methods can be used to make inference cheaper in memory or/and faster in time.
> 1. Apply various parallelism to scale up the model across a large number of GPUs. Smart parallelism of model components and data makes it possible to run a model of trillions of parameters. （批注： 例如，Deepspeed inference对dense和MoE 稀疏模型的并行策略，提高并行度，降低计算延迟）
> 2. Memory offloading to offload temporarily unused data to the CPU and read them back when needed later. This helps with memory usage but causes higher latency. （批注： 例如，flexgen和Deepspeed inference都有对CPU offload的设计，其中flexgen更是将这种设计推向新高度，核心追求throughout性能，适合离线场景）
> 3. Smart batching strategy; E.g. EffectiveTransformer packs consecutive sequences together to remove padding within one batch.
> 4. Network compression techniques, such as pruning, quantization, distillation. A model of smaller size, in terms of parameter count or bitwidth, should demand less memory and run faster. （批注： 一般牺牲精度或者需要微调，在小模型时代端侧推理常用的方法，现在在大模型时代，这种类似优化技巧在云端也更加重视）
> 5. Improvement specific to a target model architecture. Many architectural changes, especially those for attention layers, help with transformer decoding speed. （批注： Large Transformer Model Inference Optimization 重点总结了模型结构方面的优化设计，例如，围绕Transformer模型结构进行计算优化，降低理论计算量，不是计算机系统方面的优化设计了）

