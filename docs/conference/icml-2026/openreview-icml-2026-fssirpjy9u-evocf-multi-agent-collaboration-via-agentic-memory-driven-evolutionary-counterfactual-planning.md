---
title: "EvoCF: Multi-Agent Collaboration via Agentic Memory-Driven Evolutionary Counterfactual Planning"
title_zh: EvoCF：基于智能体记忆驱动进化反事实规划的多智能体协作
authors: "Haotian Chi, Zeyu Feng, Xingrui Yu, Linbo Luo, Yew-Soon Ong, Ivor Tsang, Hechang Chen, Yi Chang, Haiyan Yin"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9fad72d7b7bbe2d670d065bff44b04133136bbb2.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 基于失败归纳的演化规则库进行进化式反事实规划
tldr: 针对LLM规划器难以捕捉真实环境中物理与协调约束、多智能体协作策略难以优化的挑战，本文提出EvoCF框架。该方法先用符号约束归纳器从失败中提炼可复用规则形成演化规则库，再通过规则条件化的进化反事实规划生成并评估语义一致的方案变体。实验表明该框架能发现改进的多智能体协作策略。这为智能体协作行为的进化优化提供了新途径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM规划器难以捕捉真实环境中多智能体系统的物理与协调约束。
method: 提出EvoCF，用符号约束归纳器构建演化规则库并进行规则条件化进化反事实规划。
result: 该框架通过反事实方案生成与评估发现更优的多智能体协作策略。
conclusion: 进化反事实规划为智能体协作行为的持续优化提供了有效方法。
---

## Abstract
Planning collaboration strategies for multi-agent embodied systems remains a core challenge for LLM-based planners, which often fail to capture the physical and coordination constraints of realworld environments. To address this, we present EvoCF, an agentic memory-driven evolutionary counterfactual planning framework for discovering improved multi-agent collaboration strategies through counterfactual plan generation and evaluation. First, we propose a symbolic constraint inductor that induces reusable symbolic constraints from failures, forming an evolving rule library. Then, we propose an evolutionary counterfactual plan generator that systematically explores semantically consistent plan variants through rule-conditioned mutations, enabling robust collaboration strategies beyond short-sighted one-shot LLM plans. Finally, we design an agentic memory-grounded evaluator that ranks candidate plans using retrieval-augmented evidence, producing interpretable, constraint-aware selections. Across multi-agent embodied simulation benchmarks, EvoCF consistently discovers more robust and executable plans compared to baseline approaches. Our results demonstrate that grounding multi-agent planning in agentic memory and counterfactual reasoning significantly enhances both effectiveness and robustness.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
基于失败归纳的演化规则库进行进化式反事实规划。

### 2. 核心内容
针对LLM规划器难以捕捉真实环境中物理与协调约束、多智能体协作策略难以优化的挑战，本文提出EvoCF框架。该方法先用符号约束归纳器从失败中提炼可复用规则形成演化规则库，再通过规则条件化的进化反事实规划生成并评估语义一致的方案变体。实验表明该框架能发现改进的多智能体协作策略。这为智能体协作行为的进化优化提供了新途径。

### 3. 对应检索需求
evolutionary algorithms for evolving agent behaviors and architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=FsSirPJy9U](https://openreview.net/forum?id=FsSirPJy9U)
