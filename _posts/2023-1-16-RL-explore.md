---
title: 'Explore for some Topic about Distribute RL and HPC'
tags: RL Explore
---

<!--more-->

# RLlib

- Challenge

	- Because of the absence of a single dominant computational pattern  or fundamental rules of composition, the design and implementation of RL algorithms is hard for researchers.

- Insight

	- **Irregularity** of RL training workloads Modern RL algorithms are highly irregular in the computation patterns they create

		1. The duration and **resource requirements** of tasks differ by orders of magnitude depending on the algorithm
		2. **Communication** patterns vary
		3. **Nested** **computations** are generated by model-based hybrid algorithms

		4. Maintain and update substantial **amounts** of **state**

- Contribution

	- Distributing RL components in a composable way by adapting algorithms for top-down hierarchical control, thereby encapsulating **parallelism** and resource requirements within short-running compute tasks.
	- These primitives enable a broad range of algorithms to be implemented with **high performance**, scalability, and **substantial code reuse**.

- See more details in ...




# Distributed RL (Algorithm)


# Muti-Agent RL

#### MARLLIB: Extending Rllib For Multi-agent Reinforcement Learning

> https://arxiv.org/abs/2210.13708

- MARLlib manages to unify tens of algorithms, including different types of independent learning, centralized critic, and value decomposition methods; this leads to a highly composable integration of MARL algorithms that are not possible to unify before.    
- Furthermore, MARLlib goes beyond current work by integrating diverse environment interfaces and providing flexible parameter sharing strategies;    this allows to create versatile solutions to cooperative, competitive, and mixed tasks with minimal code modifications for end users.    
- A plethora of experiments are conducted to substantiate the correctness of our implementation, based on which we further derive new insights on the relationship between the performance and the design of algorithmic components.

Exploration in Deep Reinforcement Learning: From Single-Agent to Multi-Agent Domain

> https://arxiv.org/abs/2109.06668

Distributed Deep Reinforcement Learning: A Survey and A Multi-Player Multi-Agent Learning Toolbox

> https://arxiv.org/abs/2212.00253


# RL for HPC

DRAS-CQSim: A Reinforcement Learning based Framework for HPC Cluster Scheduling

> https://arxiv.org/abs/2105.07526

Analyzing I/O Performance of a Hierarchical HPC Storage System for Distributed Deep Learning

> https://arxiv.org/abs/2301.01494

Review, Analysis and Design of a Comprehensive Deep Reinforcement Learning Framework

> https://arxiv.org/abs/2002.11883

# Other RL
Reincarnating Reinforcement Learning: Reusing Prior Computation to Accelerate Progress

https://agarwl.github.io/reincarnating_rl/
