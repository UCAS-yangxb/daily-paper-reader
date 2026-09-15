---
title: "ALSO: Adversarial Online Strategy Optimization for Social Agents"
title_zh: ALSO：面向社交智能体的对抗在线策略优化
authors: "Xiang Li, Liping Yi, Mingze Kong, Min Zhang, Zhongxiang Dai, Qinghua Hu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9ad2481a308e01661145e3b7814654f484c34e03.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 在线策略优化适应动态环境
tldr: 社交模拟环境本质非平稳，要求智能体随时间动态调整策略，但多数LLM社交智能体依赖静态人设，离线强化学习等方法难以适用。本文提出ALSO，首个面向社交智能体的对抗在线策略优化框架。智能体在多轮对话中实时适应变化的对手，无需大量训练开销即可提升社交智能。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 社交模拟环境非平稳，而多数LLM社交智能体依赖静态人设，离线RL等方法难以适用。
method: 提出ALSO，首个在线策略优化框架，使智能体在动态环境中实时调整策略。
result: 智能体在多轮对话中对抗性地适应变化对手，无需大量训练开销。
conclusion: 为动态环境下的智能体自适应策略提供新范式。
---

## Abstract
Social simulation provides a compelling testbed for studying social intelligence, where agents interact through multi-turn dialogues under evolving contexts and strategically adapting opponents.
Such environments are inherently non-stationary, requiring agents to dynamically adjust their strategies over time.
However, most Large Language Model (LLM) based social agents rely on static personas, while existing approaches for enhancing social intelligence, such as offline reinforcement learning or external planners, are ill-suited to these settings, typically assuming stationarity and incurring substantial training overhead.
To bridge this gap, we propose **ALSO** (**A**dversarial on**L**ine **S**trategy **O**ptimization), the first framework for online strategy optimization in multi-agent social simulation.
ALSO advances social adaptation through two key contributions.
(1) ALSO formulates multi-turn interaction as an adversarial bandit problem, where combinations of static personas and dynamic strategy instructions are treated as arms, providing a principled solution to non-stationarity without relying on environmental stability assumptions.
(2) To predict rewards and generalize sparse feedback in multi-turn dialogues, ALSO introduces a lightweight neural surrogate to predict rewards from interaction histories, enabling sample-efficient exploration and continuous online adaptation.
Experiments on the Sotopia benchmark demonstrate that ALSO consistently outperforms static baselines and existing optimization methods in dynamic environments, validating the effectiveness of adversarial online strategy optimization for building robust social agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
在线策略优化适应动态环境。

### 2. 核心内容
社交模拟环境本质非平稳，要求智能体随时间动态调整策略，但多数LLM社交智能体依赖静态人设，离线强化学习等方法难以适用。本文提出ALSO，首个面向社交智能体的对抗在线策略优化框架。智能体在多轮对话中实时适应变化的对手，无需大量训练开销即可提升社交智能。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=OAvNOSbhwL](https://openreview.net/forum?id=OAvNOSbhwL)
