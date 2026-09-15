---
title: Offline Multi-agent Continual Cooperation via Skill Partition and Reuse
title_zh: 基于技能划分与复用的离线多智能体持续协作
authors: "Yuchen Xiao, Lei Yuan, Ruiqi Xue, Tieyue Yin, Yang Yu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/0dc5f123a5a55a551e3fe7fb8a07ed7dc48dd573.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 持续发现与复用技能以克服灾难性遗忘
tldr: 针对任务顺序出现、技能空间指数增长时固定技能库易受分布偏移与干扰、出现灾难性遗忘与可塑性丧失的问题，本文提出持续离线多智能体框架COMAD。该方法通过技能划分与复用从混合多智能体数据中发现协调技能，使智能体在开放环境中持续发现并复用技能。实验表明该框架能缓解遗忘并保持学习可塑性，为多智能体的终身持续协作提供了有效途径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 任务顺序出现时固定技能库面临分布偏移、灾难性遗忘与可塑性丧失。
method: 提出COMAD，通过技能划分与复用从离线数据中持续发现协调技能。
result: 缓解灾难性遗忘并保持学习可塑性，支持开放环境下的持续协作。
conclusion: 为多智能体在动态任务序列中的终身持续学习提供了有效框架。
---

## Abstract
Extracting skills from multi-agent offline dataset improves learning efficiency via sharing task-invariant coordination skills among tasks. In settings where tasks occur sequentially and the space of skills grows exponentially, existing approaches that rely on heuristically designed and fixed-sized skill libraries struggle to resolve the problem of distributional shift and interference, facing catastrophic forgetting and plasticity loss. To address this problem and endow agents with the ability to continually discover and reuse coordination skills in open-environment, we propose COMAD, a principled framework for **C**ontinual **O**ffline **M**ulti-**a**gent Skill **D**iscovery via Skill Partition and Reuse. We first discover skills from mixed multi-agent behavior data with an auto-encoder to transform coordination knowledge into reusable coordination skills. Then we construct a skill-augmented policy learning objective with multi-head architectures, explicitly guiding the advantage function with reusable skills identified via a density-based reusability estimator.
Theoretical analysis shows our method approximates the optimum of a continual skill discovery problem. Empirical results across diverse MARL benchmarks show that COMAD continually expands its skill library to mitigate interference, achieving superior forward and backward transfer for task streams compared to multiple baselines.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
持续发现与复用技能以克服灾难性遗忘。

### 2. 核心内容
针对任务顺序出现、技能空间指数增长时固定技能库易受分布偏移与干扰、出现灾难性遗忘与可塑性丧失的问题，本文提出持续离线多智能体框架COMAD。该方法通过技能划分与复用从混合多智能体数据中发现协调技能，使智能体在开放环境中持续发现并复用技能。实验表明该框架能缓解遗忘并保持学习可塑性，为多智能体的终身持续协作提供了有效途径。

### 3. 对应检索需求
lifelong learning and continual adaptation in artificial agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=5kteupXJ7B](https://openreview.net/forum?id=5kteupXJ7B)
