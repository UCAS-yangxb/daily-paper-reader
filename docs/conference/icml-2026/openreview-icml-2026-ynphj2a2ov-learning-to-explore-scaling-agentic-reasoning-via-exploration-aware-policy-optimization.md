---
title: "Learning to Explore: Scaling Agentic Reasoning via Exploration-Aware Policy Optimization"
title_zh: 学会探索：通过探索感知策略优化扩展智能体推理
authors: "Xingyuan Hua, Sheng Yue, Ju Ren"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/1eaaa70094a1d7c3a9a83f5516f18234624bca0c.pdf"
tags: ["query:self-evolve"]
score: 4.0
evidence: 自适应探索策略使智能体依据不确定性决定何时探索
tldr: 针对智能体测试时扩展中探索策略缺乏区分、无法自适应判断何时需要探索的问题，本文提出探索感知的强化学习框架。该方法通过变分推断设计细粒度奖励函数，评估探索性动作对未来决策的潜在收益，并结合探索感知分组机制。实验表明智能体能在高不确定性时自适应探索，提升推理与决策表现。这为智能体在动态环境中的自适应行为提供了机制支持。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有智能体测试时扩展采用无差别探索策略，无法自适应判断何时需要探索。
method: 提出探索感知强化学习框架，用变分推断奖励评估探索动作并分组区分探索。
result: 智能体能在高不确定性时自适应探索，提升未来决策与推理表现。
conclusion: 探索感知策略为智能体在动态环境中的自适应决策提供了有效机制。
---

## Abstract
Recent advancements in agentic test-time scaling allow models to gather environmental feedback before committing to final actions. A key limitation of existing methods is that they typically employ undifferentiated exploration strategies, lacking the ability to adaptively distinguish when exploration is truly required. In this paper, we propose an exploration-aware reinforcement learning framework that enables LLM agents to adaptively explore only when uncertainty is high. Our method introduces a fine-grained reward function via variational inference that explicitly evaluates exploratory actions by estimating their potential to improve future decision-making, together with an exploration-aware grouping mechanism that separates exploratory actions from task-completion actions during optimization. By targeting informational gaps, this design allows agents to explore selectively and transition to execution as soon as the task context is clear. Empirically, we demonstrate that our approach achieves consistent improvements across a range of challenging text-based and GUI-based agent benchmarks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自适应探索策略使智能体依据不确定性决定何时探索。

### 2. 核心内容
针对智能体测试时扩展中探索策略缺乏区分、无法自适应判断何时需要探索的问题，本文提出探索感知的强化学习框架。该方法通过变分推断设计细粒度奖励函数，评估探索性动作对未来决策的潜在收益，并结合探索感知分组机制。实验表明智能体能在高不确定性时自适应探索，提升推理与决策表现。这为智能体在动态环境中的自适应行为提供了机制支持。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=YNPHJ2A2oV](https://openreview.net/forum?id=YNPHJ2A2oV)
