---
title: Self-evolving LLM agents with in-distribution Optimization
title_zh: 基于分布内优化的自进化大模型智能体
authors: "Yudi Zhang, Meng Fang, Zhenfang Chen, Mykola Pechenizkiy"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/e51250bd0bc31fb1adf79dda5d60ea2289150131.pdf"
tags: ["query:self-evolve"]
score: 9.0
evidence: 统一过程奖励标注与策略学习的自进化LLM智能体框架
tldr: 针对LLM智能体在长时程决策中面临延迟奖励与信用分配困难的问题，本文提出自进化框架Q-Evolve。该框架在分布内强化学习范式下统一了自动过程奖励标注与策略学习，每轮迭代从混合离策略数据中学习分布内评论家，从而在稀疏奖励下稳定贝尔曼备份。实验表明该方法能有效提升智能体的长时程决策能力，为自进化LLM智能体提供了稳定的训练框架。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM智能体长时程决策中面临延迟奖励与信用分配困难。
method: 提出Q-Evolve，在分布内强化学习下统一过程奖励标注与策略学习。
result: 通过分布内评论家稳定稀疏奖励下的贝尔曼备份，提升长时程决策表现。
conclusion: 为自进化LLM智能体提供了稳定且可迭代的强化学习训练框架。
---

## Abstract
Large Language Models (LLMs) have recently emerged as powerful controllers for interactive agents in complex environments, yet training them to perform reliable long-horizon decision making remains a fundamental challenge. A key difficulty lies in credit assignment: agents often receive delayed rewards only at the end of episodes. In this paper, we propose Q-Evolve, a self-evolving framework for LLM agents that unifies automatic process-reward labeling and policy learning within a principled in-distribution reinforcement learning paradigm. In each evolving iteration, our method learns an in-distribution critic from a hybrid off-policy dataset that combines expert demonstrations with agent-generated trajectories, stabilizing Bellman backups in sparse-reward settings via a weighted Implicit Q-Learning objective. The learned value function is then used to derive step-wise process rewards through advantage estimation, enabling dense and reliable supervision without environment backtracking or human annotation. Leveraging these signals, we perform behavior-proximal policy optimization that evolves the agent over the data used for process reward labeling, allowing iterative self-improvement without exacerbating distribution shift.
We evaluate our method on AlfWorld, WebShop, and ScienceWorld, showing Q-Evolve outperforms strong baselines in sample efficiency, robustness, and overall task performance. Our results demonstrate that stable agent self-evolution is achievable through the co-evolution of process-level supervision and policy, both grounded within a shared in-distribution learning loop.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
统一过程奖励标注与策略学习的自进化LLM智能体框架。

### 2. 核心内容
针对LLM智能体在长时程决策中面临延迟奖励与信用分配困难的问题，本文提出自进化框架Q-Evolve。该框架在分布内强化学习范式下统一了自动过程奖励标注与策略学习，每轮迭代从混合离策略数据中学习分布内评论家，从而在稀疏奖励下稳定贝尔曼备份。实验表明该方法能有效提升智能体的长时程决策能力，为自进化LLM智能体提供了稳定的训练框架。

### 3. 对应检索需求
large language model based agents with self-evolution capabilities。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=kXGolRT8YX](https://openreview.net/forum?id=kXGolRT8YX)
