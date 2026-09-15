---
title: Decentralized and Disentangled Task–Role Representation Learning for Generalizable Offline Multi-Agent Meta Reinforcement Learning
title_zh: 面向可泛化离线多智能体元强化学习的去中心化解耦任务-角色表示学习
authors: "Lei Yuan, Ruiqi Xue, Yang Yu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/1adc1ded503e9b969fca4dda5316059565716529.pdf"
tags: ["query:self-evolve"]
score: 4.0
evidence: 面向快速适应的元强化学习
tldr: 离线元强化学习需从多任务数据中学习统一策略以泛化到分布外任务，但扩展到多智能体时面临去中心化任务识别困难与角色信息缺失导致的知识迁移低效。作者提出基于上下文的元强化学习框架D2TR，实现去中心化解耦的任务-角色识别。实验表明该方法提升了对分布外任务的泛化与知识迁移效率。该工作为多智能体元学习的快速适应提供了有效表示。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 离线元强化学习扩展到多智能体时面临去中心化任务识别困难与角色信息缺失导致的知识迁移低效问题。
method: 提出基于上下文的元强化学习框架D2TR，实现去中心化解耦的任务-角色识别与表示学习。
result: 提升了对分布外任务的泛化能力与知识迁移效率。
conclusion: 为多智能体元学习的快速适应提供了有效的表示方法。
---

## Abstract
Offline meta reinforcement learning (RL) enables agents to learn a unified policy from multi-task offline data to support generalization in out-of-distribution (OOD) tasks. 
Recent approaches in single-agent RL tackle this by learning an efficient task representation to distinguish between tasks, showing promising adaptation ability.
However, when extended to multi-agent settings, these methods struggle with decentralized task identification due to limited global information, and suffer from inefficient knowledge transfer in the absence of role information.
To address this, we propose D$^2$TR, a novel context-based meta RL framework with efficient decentralized and disentangled task-role identification.
Specifically, D$^2$TR first introduces mutual information knowledge distillation to align decentralized task representations with centralized task representations inferred from global trajectories, enabling efficient decentralized team-centric information identification. Next, D$^2$TR leverages a large language model to assign semantic roles to trajectories in offline data, and achieves effective individual-centric information inference by learning decentralized role representations.
Extensive experiments conducted on commonly used multi-agent environments, including CN, SMAC, and SMACv2, demonstrate that D$^2$TR exhibits strong generalization performance to unseen tasks, outperforming prior multi-agent multi-task and context-based meta RL baselines.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向快速适应的元强化学习。

### 2. 核心内容
离线元强化学习需从多任务数据中学习统一策略以泛化到分布外任务，但扩展到多智能体时面临去中心化任务识别困难与角色信息缺失导致的知识迁移低效。作者提出基于上下文的元强化学习框架D2TR，实现去中心化解耦的任务-角色识别。实验表明该方法提升了对分布外任务的泛化与知识迁移效率。该工作为多智能体元学习的快速适应提供了有效表示。

### 3. 对应检索需求
self improvement and meta learning techniques for evolving agent behaviors。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=rv1vx7zf2U](https://openreview.net/forum?id=rv1vx7zf2U)
