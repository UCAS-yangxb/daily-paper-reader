---
title: Neuro-evolutionary Continual Reinforcement Learning
title_zh: 神经进化持续强化学习
authors: "Pengyi Li, Hongyao Tang, Yifu Yuan, YAN ZHENG, Xin Xu, Jianye HAO"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/718ba942b4a3f03d972afafbae6506c462828e20.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 神经进化持续强化学习，进化掩码种群
tldr: 在开放式真实环境中部署机器人需要持续学习能力，既要保留旧技能又要利用先验知识学习新任务。受神经科学启发，本文提出神经进化持续强化学习Nevo-CRL，维护固定容量单体策略网络，通过优化层间连接与神经元参数求解任务，并为每个新任务构造掩码种群选择性激活各隐藏层输出。完成每个任务后保存最佳掩码，从而在任务不断扩展时保留并复用技能，实现无遗忘的持续适应。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 开放式环境中机器人需持续学习，既要保留旧技能又要利用先验学习新任务。
method: 提出Nevo-CRL，用掩码种群进化式激活固定容量策略网络以形成任务特定策略。
result: 保存最佳掩码使智能体在任务扩展时保留并复用技能，缓解遗忘。
conclusion: 将神经进化与持续强化学习结合，实现无遗忘的持续适应。
---

## Abstract
Deploying robots in open-ended real-world environments demands continual learning capabilities to adapt to an ever-expanding range of tasks. This requires retaining previously acquired skills without forgetting while effectively leveraging prior knowledge to learn new ones. Inspired by neuroscience, we propose **N**euro-**e**volutionary **C**ontinual **R**einforcement **L**earning (**Nevo-CRL**). Nevo-CRL maintains a fixed-capacity monolithic policy network, solving tasks by optimizing inter-layer connectivity and neuron parameters.
For each new task, Nevo-CRL constructs a mask population to selectively activate the outputs of each hidden layer, thereby forming a task-specific policy population. Upon completing each task, the best-performing mask is stored, and its activated neurons are frozen to prevent catastrophic forgetting. To facilitate knowledge transfer, Nevo-CRL reuses neurons from acquired skills based on semantic similarity between tasks, while dynamically allocating additional neurons for task-specific adaptation.
In the learning process, Nevo-CRL iteratively adjusts masks via importance-guided crossover to optimize the policy network connectivity. To improve neuron utilization, we prune low-activity connections to recycle neurons. Experiments demonstrate that Nevo-CRL achieves state-of-the-art performance among continual RL methods.
The code is available at [https://github.com/yeshenpy/Nevo-CRL](https://github.com/yeshenpy/Nevo-CRL).

---

## 论文详细总结（自动生成）

### 1. 检索相关性
神经进化持续强化学习，进化掩码种群。

### 2. 核心内容
在开放式真实环境中部署机器人需要持续学习能力，既要保留旧技能又要利用先验知识学习新任务。受神经科学启发，本文提出神经进化持续强化学习Nevo-CRL，维护固定容量单体策略网络，通过优化层间连接与神经元参数求解任务，并为每个新任务构造掩码种群选择性激活各隐藏层输出。完成每个任务后保存最佳掩码，从而在任务不断扩展时保留并复用技能，实现无遗忘的持续适应。

### 3. 对应检索需求
evolutionary algorithms for evolving agent behaviors and architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=Hv0jK8xYcT](https://openreview.net/forum?id=Hv0jK8xYcT)
