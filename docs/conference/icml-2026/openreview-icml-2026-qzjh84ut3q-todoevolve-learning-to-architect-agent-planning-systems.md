---
title: "TodoEvolve: Learning to Architect Agent Planning Systems"
title_zh: TodoEvolve：学习构建智能体规划系统
authors: "Jiaxi Liu, Guibin Zhang, Yanzuo Jiang, Zihan Zhang, Heng Chang, Zhenfei Yin, Qibing Ren, Junchi Yan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/edc35abd0a8ed76f34162fb5481ab1759eaebc3f.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 元规划范式自主合成并动态修正任务特定的规划架构
tldr: 针对现有智能体规划依赖固定手工结构、难以适应开放问题结构多样性的问题，本文提出TodoEvolve元规划范式。该方法构建PlanFactory模块化设计空间，统一拓扑、初始化、适应与导航等规划要素，使智能体能够自主合成并动态修正任务特定的规划架构。实验表明该范式可提升对多样化开放任务的适应能力。这为智能体规划系统的自我进化提供了元学习式路径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有智能体规划依赖固定手工结构，难以适应开放问题的结构多样性。
method: 提出TodoEvolve元规划范式与PlanFactory设计空间，自主合成并修正任务特定规划架构。
result: 该方法使智能体能够动态生成适配不同任务的规划结构。
conclusion: 元规划为智能体规划系统的自主进化与适应提供了新范式。
---

## Abstract
Planning has become a central capability for contemporary agent systems in navigating complex, long-horizon tasks, yet existing approaches predominantly rely on fixed, hand-crafted planning structures that lack the flexibility to adapt to the structural diversity of open-ended problems. To address this limitation, we introduce TodoEvolve, a meta-planning paradigm that autonomously synthesizes and dynamically revises task-specific planning architectures. Specifically, we first construct PlanFactory, a modular design space that standardizes diverse planning paradigms within a unified codebase encompassing topology, initialization, adaptation, and navigation, thereby providing a common interface for heterogeneous planning patterns. Leveraging PlanFactory, we collect high-quality planning trajectories and train Todo-14B via Impedance-Guided Preference Optimization (IGPO), a multi-objective reinforcement learning objective that encourages the generation of planning systems that are performant, stable, and token-efficient across arbitrary tasks and agent backbones. Empirical evaluations on five agentic benchmarks demonstrate that TodoEvolve consistently surpasses carefully engineered planning modules while maintaining economical API costs and runtime overhead. Our codes are available at \url{https://github.com/EcthelionLiu/TodoEvolve}.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
元规划范式自主合成并动态修正任务特定的规划架构。

### 2. 核心内容
针对现有智能体规划依赖固定手工结构、难以适应开放问题结构多样性的问题，本文提出TodoEvolve元规划范式。该方法构建PlanFactory模块化设计空间，统一拓扑、初始化、适应与导航等规划要素，使智能体能够自主合成并动态修正任务特定的规划架构。实验表明该范式可提升对多样化开放任务的适应能力。这为智能体规划系统的自我进化提供了元学习式路径。

### 3. 对应检索需求
self improvement and meta learning techniques for evolving agent behaviors。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=QZjH84ut3Q](https://openreview.net/forum?id=QZjH84ut3Q)
