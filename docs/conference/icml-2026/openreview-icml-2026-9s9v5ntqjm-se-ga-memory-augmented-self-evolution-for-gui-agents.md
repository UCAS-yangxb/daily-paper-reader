---
title: "SE-GA: Memory-Augmented Self-Evolution for GUI Agents"
title_zh: SE-GA：面向GUI智能体的记忆增强自进化
authors: "Shilong Jin, Lanjun Wang, Zhuosheng Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/08ac4b5e4ff21fb40631ba5b306f6542c6784e16.pdf"
tags: ["query:self-evolve"]
score: 9.0
evidence: 带迭代自改进的自进化GUI智能体
tldr: GUI智能体受限于上下文窗口与静态策略，难以适应动态环境中的多步任务。本文提出SE-GA，融合分层记忆与迭代自改进机制，包含测试时记忆扩展与记忆增强自进化训练流程。它通过动态检索情景、语义与经验记忆支撑长期规划，并利用收集数据持续稳定地自我进化，为GUI智能体提供持续适应框架。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: GUI智能体受限于上下文窗口与静态策略，难以适应动态环境中的多步任务。
method: 提出SE-GA，融合分层记忆与迭代自改进，含测试时记忆扩展与记忆增强自进化训练流程。
result: 通过动态检索情景、语义与经验记忆支撑长期规划并持续学习。
conclusion: 为GUI智能体提供持续适应与自我进化框架。
---

## Abstract
Autonomous Graphical User Interface (GUI) agents often struggle with multi-step tasks due to constrained context windows and static policies that fail to adapt to dynamic environments. To address these limitations, this work proposes the Self-Evolving GUI Agent (SE-GA), a novel framework that integrates hierarchical memory structures with an iterative self-improvement mechanism.  At the core of our approach is Test-Time Memory Extension (TTME), which facilitates long-term planning by dynamically retrieving episodic, semantic, and experiential memories to provide salient contexts during inference. To ensure continuous learning, we introduce Memory-Augmented Self-Evolution (MASE), which is a training pipeline that adopts the data collected by TTME to stabilize and enhance the agent's foundational policy. Extensive evaluations across both offline and online benchmarks demonstrate SE-GA achieves state-of-the-art performance, reaching success rates of 89.0\% on ScreenSpot and 75.8\% on the challenging AndroidControl-High dataset. Furthermore, significant improvements on the AndroidWorld benchmark highlight the superior generalization to dynamic environments.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
带迭代自改进的自进化GUI智能体。

### 2. 核心内容
GUI智能体受限于上下文窗口与静态策略，难以适应动态环境中的多步任务。本文提出SE-GA，融合分层记忆与迭代自改进机制，包含测试时记忆扩展与记忆增强自进化训练流程。它通过动态检索情景、语义与经验记忆支撑长期规划，并利用收集数据持续稳定地自我进化，为GUI智能体提供持续适应框架。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=9S9V5ntQJM](https://openreview.net/forum?id=9S9V5ntQJM)
