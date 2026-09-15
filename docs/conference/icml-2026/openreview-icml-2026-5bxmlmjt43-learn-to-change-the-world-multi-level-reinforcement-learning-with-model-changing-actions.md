---
title: "Learn to change the world: Multi-level reinforcement learning with model-changing actions"
title_zh: 学会改变世界：具有模型改变动作的多层强化学习
authors: "Ziqing Lu, Babak Hassibi, Lifeng Lai, Weiyu Xu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/316d60d574dd0e8a2310e72cd4e55e84b7891886.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 具模型改变动作的智能体
tldr: 传统强化学习假设环境固定，智能体只能被动适应。本文考虑具有模型改变动作的智能体，提出多层可配置时变马尔可夫决策过程，使智能体通过上层动作重配置底层的非平稳转移函数。智能体可主动重构世界动力学以提升奖励，拓展了智能体主动适应与自我改变环境的能力边界。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 传统RL假设环境固定，智能体仅被动适应，无法主动改变世界动态。
method: 提出多层可配置时变MDP，智能体通过上层模型改变动作重配置底层转移函数。
result: 智能体可主动重构环境动力学以提升奖励。
conclusion: 拓展了智能体主动适应与自我改变环境的能力边界。
---

## Abstract
Reinforcement learning usually assumes a given or sometimes even fixed environment in which an agent seeks an optimal policy to maximize its long-term discounted reward. In contrast, we consider agents that are not limited to passive adaptations: they instead have model-changing actions that actively modify the RL model of world dynamics itself. Reconfiguring the underlying transition processes can potentially increase the agents' rewards. Motivated by this setting, we introduce the multi-layer configurable time-varying Markov decision process (MCTVMDP). In an MCTVMDP, the lower-level MDP has a non-stationary transition function that is configurable through upper-level model-changing actions. The agent's objective consists of two parts: Optimize the configuration policies in the upper-level MDP and optimize the primitive action policies in the lower-level MDP to jointly improve its expected long-term reward.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
具模型改变动作的智能体。

### 2. 核心内容
传统强化学习假设环境固定，智能体只能被动适应。本文考虑具有模型改变动作的智能体，提出多层可配置时变马尔可夫决策过程，使智能体通过上层动作重配置底层的非平稳转移函数。智能体可主动重构世界动力学以提升奖励，拓展了智能体主动适应与自我改变环境的能力边界。

### 3. 对应检索需求
evolutionary algorithms for evolving agent behaviors and architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=5BXMlmjt43](https://openreview.net/forum?id=5BXMlmjt43)
