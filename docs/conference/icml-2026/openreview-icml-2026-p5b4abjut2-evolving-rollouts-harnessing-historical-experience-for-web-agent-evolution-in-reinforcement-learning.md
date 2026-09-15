---
title: "EVOLVING ROLLOUTS: Harnessing Historical Experience for Web Agent Evolution in Reinforcement Learning"
title_zh: 进化轨迹：利用历史经验推动网页智能体在强化学习中进化
authors: "Sinuo Wang, WANG PIAOHONG, Tianrui Qin, Maojia Song, Qianben Chen, Qiexiang Wang, Gengze Zhou, Zeyu Zhang, He Zhu, Dingfeng Shi, Yutong Xie, Minghao Liu, Jiaheng Liu, Ge Zhang, Jiawei Ma, Yuchen Eleanor Jiang, Qi Wu, Wangchunshu Zhou"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/1d88b708e565a2d9713f10f498733357b2a6e306.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 将轨迹蒸馏为经验以推动网页智能体在强化学习中进化
tldr: 针对网页搜索智能体强化学习成本高昂、且基于分组的优化丢弃零方差组学习信号的问题，本文提出EVOLVING ROLLOUTS框架。该方法将带奖励标注的轨迹蒸馏为策略经验，作为上下文引导注入未来行为，从而在参数空间优化之外增加隐式的上下文空间优化。实验表明该框架能使智能体持续利用历史经验进化，提升训练效率与性能，为智能体的经验驱动自进化提供了新机制。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 网页智能体强化学习代价高，分组优化会丢弃零方差组的学习信号。
method: 提出EVOLVING ROLLOUTS，将带奖励轨迹蒸馏为上下文经验并优化策略行为。
result: 在参数空间优化外引入上下文空间优化，提升训练效率与智能体表现。
conclusion: 为智能体基于历史经验的自进化提供了低成本、可复用的新机制。
---

## Abstract
Agentic reinforcement learning (RL) for web search is prohibitively expensive due to long context lengths and costly environment interactions, and this inefficiency is further exacerbated by group-based optimization, which discards learning signals from entire rollout groups with zero reward variance. In this work, we propose EVOLVING ROLLOUTS, an RL framework for web-search agents that moves beyond episodic training and distills collected rollouts into in-context guidance for future policy behavior. By extracting the reward-labeled trajectories into strategic experiences, our method augments standard parameter-space optimization with implicit context-space optimization guided by prior experience. This enables the agent to recover learning signals from zero-variance rollouts, thereby fostering co-evolution between the policy and the experience repository. EVOLVING ROLLOUTS improves sample efficiency and task performance across representative web search benchmarks, with Qwen3-8B surpassing the much larger Qwen3-30B-A3B in average performance across GAIA, xBench, and HLE, and Qwen3-4B attaining comparable results on GAIA and HLE.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
将轨迹蒸馏为经验以推动网页智能体在强化学习中进化。

### 2. 核心内容
针对网页搜索智能体强化学习成本高昂、且基于分组的优化丢弃零方差组学习信号的问题，本文提出EVOLVING ROLLOUTS框架。该方法将带奖励标注的轨迹蒸馏为策略经验，作为上下文引导注入未来行为，从而在参数空间优化之外增加隐式的上下文空间优化。实验表明该框架能使智能体持续利用历史经验进化，提升训练效率与性能，为智能体的经验驱动自进化提供了新机制。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=p5B4ABjuT2](https://openreview.net/forum?id=p5B4ABjuT2)
