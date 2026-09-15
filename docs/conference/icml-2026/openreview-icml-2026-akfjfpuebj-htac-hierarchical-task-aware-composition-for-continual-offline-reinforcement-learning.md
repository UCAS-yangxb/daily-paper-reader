---
title: "HTAC: Hierarchical Task-Aware Composition for Continual Offline Reinforcement Learning"
title_zh: HTAC：面向持续离线强化学习的分层任务感知组合
authors: "Qiyang Zhou, Xu Ruihang, Peng Wang, WenJie Lu, Xiaochun Cao, Naiqiang Tan, Li Shen"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a8a4709d6b29d7255861361745d2c2f1d73b8261.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 持续离线强化学习构建可迁移知识的长期自主智能体
tldr: 持续离线强化学习旨在用静态数据构建长期自主智能体，但任务间动态、奖励与行为策略的异质性及离线分布偏移，要求智能体在迁移时选择性复用共享知识并隔离任务特有特征，现有扁平知识共享难以做到。作者提出HTAC分层任务感知组合方法，通过双层任务编码与软组合平衡可塑性与稳定性。实验表明其改善了跨任务泛化，为智能体的持续适应提供了方法。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续离线强化学习面临任务异质性与分布偏移，扁平知识共享限制跨任务泛化。
method: 提出HTAC，用双层任务编码与软组合机制平衡可塑性与稳定性。
result: 实现共享知识的复用与任务特有特征隔离，改善跨任务泛化。
conclusion: 为长期自主智能体的持续适应提供了知识组合方法。
---

## Abstract
Continual Offline Reinforcement Learning (CORL) enables building long-term autonomous agents from static datasets. However, it faces heterogeneity in environment dynamics, reward functions, and behavior policies across tasks. Combined with the inherent distribution shift in offline learning, this requires agents to selectively reuse shared knowledge during transfer while isolating task-specific features. The flat knowledge sharing mechanisms employed by existing methods struggle to capture such distinctions, limiting cross-task generalization.
To address this, we propose Hierarchical Task-Aware Composition (HTAC), which balances plasticity and stability through dual-level task encoding and soft composition mechanisms. HTAC comprises four modules: (1) a Hierarchical Semantic Task Representation that decomposes tasks into domain-level and task-level embeddings; (2) a Dual-level Expert Network that creates domain and task experts on demand for parameter-efficient knowledge isolation; (3) an Adaptive Knowledge Composition module that integrates historical expert outputs via attention mechanisms for knowledge reuse; (4) Task Adapters that preserve historical routing weights to prevent forgetting. Experiments on Offline Continual World show that HTAC outperforms existing baselines, demonstrating better knowledge reuse and transfer capabilities.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
持续离线强化学习构建可迁移知识的长期自主智能体。

### 2. 核心内容
持续离线强化学习旨在用静态数据构建长期自主智能体，但任务间动态、奖励与行为策略的异质性及离线分布偏移，要求智能体在迁移时选择性复用共享知识并隔离任务特有特征，现有扁平知识共享难以做到。作者提出HTAC分层任务感知组合方法，通过双层任务编码与软组合平衡可塑性与稳定性。实验表明其改善了跨任务泛化，为智能体的持续适应提供了方法。

### 3. 对应检索需求
methods for lifelong learning and continual adaptation in autonomous intelligent agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=akfJfpUEBj](https://openreview.net/forum?id=akfJfpUEBj)
