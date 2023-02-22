---
title           : 'UCB: AIsys Catalogue'
image           : '2023-01-02-AIsys-index/1677075722704.png'

---

<!--more-->

> [https://ucbrise.github.io/cs294-ai-sys-sp22/](https://ucbrise.github.io/cs294-ai-sys-sp22/)

# Course Description

The recent success of AI has been in large part due in part to advances in hardware and software systems. These systems have enabled training increasingly complex models on ever larger datasets. In the process, these systems have also simplified model development, enabling the rapid growth in the machine learning community. These new hardware and software systems include a new generation of GPUs and hardware accelerators (e.g., TPU), open source frameworks such as Theano, TensorFlow, PyTorch, MXNet, Apache Spark, Clipper, Horovod, and Ray, and a myriad of systems deployed internally at companies just to name a few. At the same time, we are witnessing a flurry of ML/RL applications to improve hardware and system designs, job scheduling, program synthesis, and circuit layouts.

In this course, we will describe the latest trends in systems designs to better support the next generation of AI applications, and applications of AI to optimize the architecture and the performance of systems. The format of this course will be a mix of lectures, seminar-style discussions, and student presentations. Students will be responsible for paper readings, and completing a hands-on project. For projects, we will strongly encourage teams that contains both AI and systems students.

# Paper List

## 1. Introduction and Course Overview

### Require Reading

- - [x] [SysML: The New Frontier of Machine Learning Systems](https://arxiv.org/abs/1904.03257)
- - [x] Read Chapter 1 of [*Principles of Computer System Design*](https://www.sciencedirect.com/book/9780123749574/principles-of-computer-system-design). You will need to be on campus or use the Library VPN to obtain a free PDF.
- - [x] [A Few Useful Things to Know About Machine Learning](https://homes.cs.washington.edu/~pedrod/papers/cacm12.pdf)

### Additional Optional Reading

- - [x] [How to read a paper](https://web.stanford.edu/class/ee384m/Handouts/HowtoReadPaper.pdf) provides some pretty good advice on how to read papers effectively.
- - [x] Timothy Roscoe’s [writing reviews for systems conferences](https://people.inf.ethz.ch/troscoe/pubs/review-writing.pdf) will also help you in the reviewing process.

## 2. Big Data Systems

### Require Reading

- - [x] [Towards a Unified Architecture for in-RDBMS Analytics](https://www.cs.stanford.edu/people/chrismre/papers/bismarck.pdf)
- - [x] [Resilient Distributed Datasets: A Fault-Tolerant Abstraction for In-Memory Cluster Computing](https://www.usenix.org/system/files/conference/nsdi12/nsdi12-final138.pdf)
- - [x] [Lakehouse: A New Generation of Open Platforms that Unify Data Warehousing and Advanced Analytics](http://cidrdb.org/cidr2021/papers/cidr2021_paper17.pdf)

### Additional Optional Reading

- - [x] [Delta Lake: High-Performance ACID Table Storage over Cloud Object Stores](https://databricks.com/wp-content/uploads/2020/08/p975-armbrust.pdf)
- - [x] [Spark SQL: Relational Data Processing in Spark](https://people.csail.mit.edu/matei/papers/2015/sigmod_spark_sql.pdf)
- - [ ] [The MADlib Analytics Library or MAD Skills, the SQL](https://arxiv.org/pdf/1208.4165.pdf)


## 3. Hardware for Machine Learning

### Require Reading

- - [x] [Mixed precision training. [ICLR’18\]](https://openreview.net/pdf?id=r1gs9JgRZ)
- - [x] [Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks [SIGRAPH, 2016\]](https://dspace.mit.edu/handle/1721.1/102369)
- - [x] [Interstellar: Using Halide’s Scheduling Language to Analyze DNN Accelerators (formerly: DNN Dataflow Choice Is Overrated)](https://arxiv.org/pdf/1809.04070.pdf)
- - [x] [Gemmini: Enabling Systematic Deep-Learning Architecture Evaluation via Full-Stack Integration [Best Paper Award, DAC’21\]](https://people.eecs.berkeley.edu/~ysshao/assets/papers/genc2021-dac.pdf)

### Additional Optional Reading

- - [ ] [A New Golden Age for Computer Architecture](https://cacm.acm.org/magazines/2019/2/234352-a-new-golden-age-for-computer-architecture/fulltext)
- - [ ] [Roofline: An Insightful Visual Performance Model for Floating-Point Programs and Multicore Architectures ](https://people.eecs.berkeley.edu/~kubitron/cs252/handouts/papers/RooflineVyNoYellow.pdf)

## 4. Distributed deep learning, Part I: Systems

### Require Reading

- - [ ] [Chimera: Efficiently Training Large-Scale Neural Networks with Bidirectional Pipelines [SC’21, Best Paper finalist\]](https://arxiv.org/pdf/2107.06925.pdf)
- - [ ] [Efficient Large-Scale Language Model Training on GPU Clusters Using Megatron-LM [SC’21, Best Student Paper\]](https://arxiv.org/pdf/2104.04473.pdf)
- - [ ] [ZeRO-Infinity: Breaking the GPU Memory Wall for Extreme Scale Deep Learning [SC’21\]](https://arxiv.org/abs/2104.07857)

### Additional Optional Reading

- - [ ] [DeepSpeed: Advancing MoE inference and training to power next-generation AI scale [Blog post\]](https://www.microsoft.com/en-us/research/blog/deepspeed-advancing-moe-inference-and-training-to-power-next-generation-ai-scale/)
- - [ ] [Large Scale Distributed Deep Networks [NeurIPS’12\]](https://papers.nips.cc/paper/2012/hash/6aca97005c68f1206823815f66102863-Abstract.html)
- - [ ] [Gpipe: Efficient training of giant neural networks using pipeline parallelism [NeurIPS’19\]](https://proceedings.neurips.cc/paper/2019/file/093f65e080a295f8076b1c5722a46aa2-Paper.pdf)
- - [ ] [PipeDream: Fast and Efficient Pipeline Parallel DNN Training [SOSP’19\]](https://arxiv.org/pdf/1806.03377.pdf)

## 5. Distributed deep learning, Part II: Scaling Constraints

### Require Reading

- - [ ] [Measuring the Effects of Data Parallelism on Neural Network Training](https://arxiv.org/pdf/1811.03600.pdf)
- - [ ] [Scaling Laws for Neural Language Models [OpenAI, 2020\]](https://arxiv.org/pdf/2001.08361.pdf)
- - [ ] [Deep Learning Training in Facebook Data Centers: Design of Scale-up and Scale-out Systems](https://arxiv.org/abs/2003.09518)

### Additional Optional Reading

- - [ ] [On Large-Batch Training for Deep Learning: Generalization Gap and Sharp Minima [ICLR’16\]](https://arxiv.org/pdf/1609.04836.pdf)
- - [ ] [Train Large, Then Compress: Rethinking Model Size for Efficient Training and Inference of Transformers [ICML’20\]](https://arxiv.org/pdf/2002.11794.pdf)
- - [ ] [Large Batch Optimization for Deep Learning: Training BERT in 76 minutes [ICLR’20\]](https://arxiv.org/pdf/1904.00962.pdf)
- - [ ] [Scaling Vision Transformers](https://arxiv.org/pdf/2106.04560.pdf)

## 6. Machine learning Applied to Systems

### Require Reading

- - [ ] [The Case for Learned Index Structures [ICMD’18\]](https://arxiv.org/abs/1712.01208)
- - [ ] [Device Placement Optimization with Reinforcement Learning [ICML’17\]](https://arxiv.org/pdf/1706.04972.pdf)
- - [ ] [Neural Adaptive Video Streaming with Pensieve [SIGCOMM’17\]](https://people.csail.mit.edu/hongzi/content/publications/Pensieve-Sigcomm17.pdf)

## 7. Machine Learning Frameworks and Automatic Differentiation

### Require Reading

- - [ ] [Automatic differentiation in ML: Where we are and where we should be going](https://papers.nips.cc/paper/8092-automatic-differentiation-in-ml-where-we-are-and-where-we-should-be-going)
- - [ ] [TensorFlow: A System for Large-Scale Machine Learning](https://www.usenix.org/system/files/conference/osdi16/osdi16-abadi.pdf)
- [TVM: An Automated End-to-End Optimizing Compiler for Deep Learning](https://arxiv.org/abs/1802.04799)

## 8. Efficient Machine Learning

### Require Reading

- - [ ] [Linear Mode Connectivity and the Lottery Ticket Hypothesis](https://arxiv.org/pdf/1912.05671.pdf)
- - [ ] [Integer-only Quantization of Neural Networks for Efficient Integer-Arithmetic-Only Inference](https://arxiv.org/pdf/1712.05877.pdf)
- - [ ] [FBNet: Hardware-Aware Efficient ConvNet Design via Differentiable Neural Architecture Search](https://arxiv.org/abs/1812.03443)

### Additional Optional Reading

- - [ ] [Hessian Aware trace-Weighted Quantization of Neural Networks](https://proceedings.neurips.cc/paper/2020/file/d77c703536718b95308130ff2e5cf9ee-Paper.pdf)
- - [ ] [The state of sparsity in deep neural networks](https://arxiv.org/pdf/1902.09574.pdf)
- - [ ] [Sparsity in Deep Learning: Pruning and growth for efficient inference and training in neural networks](https://arxiv.org/pdf/2102.00554.pdf)

## 9. Fundamentals of Machine Learning in the Cloud, the Modern Data Stack

### Require Reading

- - [ ] [The Sky Above The Clouds](https://drive.google.com/file/d/16xs_-3XRym34z60-Ji4dlDwW487vOmpz/view?usp=sharing)
- - [ ] [FrugalML: How to Use ML Prediction APIs More Accurately and Cheaply](https://arxiv.org/abs/2006.07512)
- - [ ] [Pollux: Co-adaptive Cluster Scheduling for Goodput-Optimized Deep Learning](https://www.usenix.org/system/files/osdi21-qiao.pdf)

### Additional Optional Reading

- - [ ] [RubberBand: cloud-based hyperparameter tuning](https://dl.acm.org/doi/10.1145/3447786.3456245)


## 10. Benchmarking Machine Learning Workloads

### Require Reading

- - [ ] [MLPerf Training Benchmark](https://proceedings.mlsys.org/paper/2020/hash/02522a2b2726fb0a03bb19f2d8d9524d-Abstract.html)
- - [ ] [MLPerf Inference Benchmark](https://arxiv.org/pdf/1911.02549.pdf)
- - [ ] [Benchmark Analysis of Representative Deep Neural Network Architectures](https://arxiv.org/pdf/1810.00736.pdf)

## 11. Machine learning and Security

### Require Reading

- - [ ] [Communication-Efficient Learning of Deep Networks from Decentralized Data](https://arxiv.org/pdf/1602.05629.pdf)
- - [ ] [Privacy Accounting and Quality Control in the Sage Differentially Private ML Platform](https://arxiv.org/pdf/1909.01502.pdf)
- - [ ] [Robust Physical-World Attacks on Deep Learning Models](https://arxiv.org/abs/1707.08945)

### Additional Optional Reading

- - [ ] [Helen: Maliciously Secure Coopetitive Learning for Linear Models](https://people.eecs.berkeley.edu/~wzheng/helen_ieeesp.pdf)
- - [ ] [Faster CryptoNets: Leveraging Sparsity for Real-World Encrypted Inference](https://arxiv.org/abs/1811.09953)
- - [ ] [Rendered Insecure: GPU Side Channel Attacks are Practical](https://www.cs.ucr.edu/~zhiyunq/pub/ccs18_gpu_side_channel.pdf)
- - [ ] [The Algorithmic Foundations of Differential Privacy](https://www.cis.upenn.edu/~aaroth/Papers/privacybook.pdf)
- - [ ] [Federated Learning: Collaborative Machine Learning without Centralized Training Data](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html)
- - [ ] [Federated Learning at Google … A comic strip?](https://federated.withgoogle.com/)
- - [ ] [SecureML: A System for Scalable Privacy-Preserving Machine Learning](https://eprint.iacr.org/2017/396.pdf)