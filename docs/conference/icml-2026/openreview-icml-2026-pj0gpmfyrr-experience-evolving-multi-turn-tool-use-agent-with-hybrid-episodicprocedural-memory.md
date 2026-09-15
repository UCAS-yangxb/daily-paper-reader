---
title: Experience-Evolving Multi-Turn Tool-Use Agent with Hybrid Episodic–Procedural Memory
title_zh: 基于混合情景-程序记忆的经验进化多轮工具使用智能体
authors: "Sijia Li, Yuchen Huang, Zifan LIU, Zijian Li, Jingjing Fu, Lei Song, Jiang Bian, Jun Zhang, Rui Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d7b1c92eae0525a01f32380127bad444afdeabf9.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 通过记忆复用实现多轮工具使用策略的经验进化
tldr: 多轮智能体面临不断变化的决策情境，复用过往经验时完整轨迹过于具体而工具级复用又忽略上下文。本文提出混合情景-程序记忆策略H-EPM，从积累轨迹构建工具图，用反复出现的工具依赖刻画程序化套路，并在推理与训练中自适应复用部分重叠的成功经验。该方法实现多轮工具使用策略的经验进化，提升智能体在动态情境下的适应与迁移能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多轮智能体决策情境不断变化，完整轨迹过于具体而工具级复用忽略上下文。
method: 提出混合情景-程序记忆策略，从轨迹构建工具图并自适应复用部分重叠经验。
result: 实现了多轮工具使用策略的经验进化，提升动态情境下的适应与迁移。
conclusion: 通过经验进化机制增强智能体持续适应变化环境的能力。
---

## Abstract
As intents unfold and environments change, multi-turn agents face continuously shifting decision contexts. Although reusing past experience is intuitively appealing, existing approaches remain limited: full trajectories are often too context-specific to transfer, while tool-level reuse ignores the context and environment. In this paper, we introduce a hybrid episodic–procedural memory strategy (H-EPM) that enables experience-evolution of multi-turn tool-use policies, by adaptively reusing partially overlapping successful experiences in both inference and training.
Inspired by human episodic–procedural integration, we build a tool graph from accumulated trajectories, where recurring tool-to-tool dependencies capture procedural routines and each edge is augmented with a compact episodic summaries of relevant context. At inference, the agent dynamically balances episodic recall for contextual reasoning and procedural execution for routine steps.
Beyond inference, H-EPM introduces a memory-guided reinforcement learning paradigm that directly addresses a core challenge in multi-turn agent RL: ineffective exploration over long trajectories. By biasing exploration toward historically successful tool transitions, H-EPM learns a stronger policy that generalizes during inference without relying on domain-specific experience collection. Experiments show that H-EPM consistently delivers substantial inference-time gains over strong baselines across multi-turn tool-use benchmarks, reaching up to 50%+. It also boosts RL policy performance, achieving up to 40%+ improvement on out-of-distribution tasks. Our code is available at https://github.com/LISijia-dev/H-EPM.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过记忆复用实现多轮工具使用策略的经验进化。

### 2. 核心内容
多轮智能体面临不断变化的决策情境，复用过往经验时完整轨迹过于具体而工具级复用又忽略上下文。本文提出混合情景-程序记忆策略H-EPM，从积累轨迹构建工具图，用反复出现的工具依赖刻画程序化套路，并在推理与训练中自适应复用部分重叠的成功经验。该方法实现多轮工具使用策略的经验进化，提升智能体在动态情境下的适应与迁移能力。

### 3. 对应检索需求
agents capable of self-improvement and autonomous skill acquisition。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=PJ0GpmFYrR](https://openreview.net/forum?id=PJ0GpmFYrR)
