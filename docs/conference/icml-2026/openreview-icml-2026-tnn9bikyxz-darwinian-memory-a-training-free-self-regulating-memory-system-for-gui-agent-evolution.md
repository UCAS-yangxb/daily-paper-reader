---
title: "Darwinian Memory: A Training-Free Self-Regulating Memory System for GUI Agent Evolution"
title_zh: 达尔文记忆：面向GUI智能体进化的免训练自调节记忆系统
authors: "Hongze Mi, Yibo Feng, WenJie Lu, Song Cao, Jinyuan Li, Yanming Li, Xuelin Zhang, Haotian Luo, Songyang Peng, He Cui, Tengfei Tian, Jun Fang, Hua Chai, Naiqiang Tan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/db9700e3ce01368639c8b929484815d1e360f418.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 面向GUI智能体的免训练自进化记忆架构，遵循适者生存法则
tldr: 针对多模态大模型GUI智能体在长程跨应用任务中受限于上下文窗口、且静态记忆积累导致幻觉的问题，本文提出达尔文记忆系统DMS。该方法将记忆构建为遵循适者生存法则的动态生态系统，把复杂轨迹分解并自我调节，无需训练即可适应动态GUI环境。实验表明该自进化架构能缓解粒度错配与上下文污染。这为智能体记忆的持续自我进化提供了新机制。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: GUI智能体在长程跨应用任务中受限于上下文窗口，静态记忆积累引发幻觉。
method: 提出DMS，将记忆构建为遵循适者生存法则的动态生态系统并分解复杂轨迹。
result: 该免训练自进化架构缓解了粒度错配与上下文污染，适应动态GUI环境。
conclusion: 自调节记忆生态为GUI智能体的持续进化提供了有效机制。
---

## Abstract
Multimodal Large Language Model (MLLM) agents facilitate Graphical User Interface (GUI) automation but struggle with long-horizon, cross-application tasks due to limited context windows. While memory systems provide a viable solution, existing paradigms struggle to adapt to dynamic GUI environments, suffering from a granularity mismatch between high-level intent and low-level execution, and context pollution where the static accumulation of outdated experiences drives agents into hallucination.  
  To address these bottlenecks, we propose the Darwinian Memory System (DMS), a self-evolving architecture that constructs memory as a dynamic ecosystem governed by the law of "survival of the fittest." DMS decomposes complex trajectories into independent, reusable units for compositional flexibility, and implements Utility-driven Natural Selection to track survival value, actively pruning suboptimal paths and inhibiting high-risk plans. This evolutionary pressure compels the agent to derive superior strategies. Extensive experiments on real-world multi-app benchmarks validate that DMS boosts general-purpose MLLMs without training costs or architectural overhead, achieving average gains of 18.0% in success rate and 33.9% in execution stability, while reducing task latency, establishing it as an effective self-evolving memory system for GUI tasks. The implementation is available at https://anonymous.4open.science/r/DMS-C48C.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向GUI智能体的免训练自进化记忆架构，遵循适者生存法则。

### 2. 核心内容
针对多模态大模型GUI智能体在长程跨应用任务中受限于上下文窗口、且静态记忆积累导致幻觉的问题，本文提出达尔文记忆系统DMS。该方法将记忆构建为遵循适者生存法则的动态生态系统，把复杂轨迹分解并自我调节，无需训练即可适应动态GUI环境。实验表明该自进化架构能缓解粒度错配与上下文污染。这为智能体记忆的持续自我进化提供了新机制。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tNn9bikyXZ](https://openreview.net/forum?id=tNn9bikyXZ)
