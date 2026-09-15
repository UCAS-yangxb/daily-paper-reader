---
title: Behavior-Invariant Task Representation Learning with Transformer-based World Models for Offline Meta-Reinforcement Learning
title_zh: 面向离线元强化学习的Transformer世界模型行为不变任务表示学习
authors: "Fuyuan Qian, Menglong Zhang, Song Wang, Quanying Liu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/4486daaf85f4b617203363acf8f5b8f3069ee831.pdf"
tags: ["query:self-evolve"]
score: 6.0
evidence: 元学习适应与任务表示学习
tldr: 离线元强化学习面临上下文与策略分布偏移，稀疏奖励下智能体难以稳健泛化到未见环境。本文融合信息论任务表示学习与Transformer随机世界模型，提取任务潜在变量。方法缓解了内在模式困境，提升智能体对在线环境的适应与泛化能力，为元学习适应提供新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 离线元RL面临上下文与策略分布偏移，稀疏奖励下难以稳健泛化到未见环境。
method: 融合信息论任务表示学习与Transformer随机世界模型，提取任务潜在变量。
result: 缓解模式困境，提升对未见环境的泛化与适应能力。
conclusion: 为智能体元学习适应提供表示学习方法。
---

## Abstract
Offline meta-reinforcement learning leverages static datasets to enable agents to generalize to unseen environments by combining offline efficiency with meta-learning adaptability, yet it faces key challenges from context and policy distribution shifts. These issues hinder agents from adapting to online environments, and are further exacerbated under sparse-reward settings. As a result, agents often become trapped in an inherent pattern dilemma, failing to achieve robust generalization. In this work, we propose a novel framework that integrates information-theoretic task representation learning with a Transformer-based stochastic world model. Our approach extracts task-defining latent variables that are invariant to behavior policy, thereby effectively mitigating the context distribution shift. To further handle policy shift and model exploitation, we apply a conservative value penalty to imagination-based rollouts, preventing the policy from exploiting model inaccuracies while maintaining robust adaptation. Extensive evaluations demonstrate that our method outperforms state-of-the-art approaches, with superior stability and generalization under out-of-distribution and sparse-reward settings.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
元学习适应与任务表示学习。

### 2. 核心内容
离线元强化学习面临上下文与策略分布偏移，稀疏奖励下智能体难以稳健泛化到未见环境。本文融合信息论任务表示学习与Transformer随机世界模型，提取任务潜在变量。方法缓解了内在模式困境，提升智能体对在线环境的适应与泛化能力，为元学习适应提供新思路。

### 3. 对应检索需求
self improvement and meta learning techniques for evolving agent behaviors。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=n4SsjVKXWQ](https://openreview.net/forum?id=n4SsjVKXWQ)
