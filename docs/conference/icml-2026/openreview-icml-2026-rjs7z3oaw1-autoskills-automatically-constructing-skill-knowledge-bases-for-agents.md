---
title: "AutoSkills: Automatically Constructing Skill Knowledge Bases for Agents"
title_zh: AutoSkills：为智能体自动构建技能知识库
authors: "Chenxi Wang, Zhuoyun Yu, Xin Xie, Wuguannan YAO, Runnan Fang, Shuofei Qiao, Kexin Cao, Guozhou Zheng, Xiang Qi, Peng Zhang, Shumin Deng"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f79dafaf2db2ffad65376badc6fc56b450e70c63.pdf"
tags: ["query:self-evolve"]
score: 9.0
evidence: 自主构建即插即用技能库
tldr: 现有自进化范式迫使每个智能体孤立学习，冗余挖掘自身有限经验，导致技能难以泛化。AutoSkills提出全自动流水线，通过多层技能设计、迭代技能精炼等机制预构建即插即用的技能库，将原始轨迹蒸馏为策略、功能与原子三级技能。该框架打破孤立学习循环，显著提升智能体技能获取的效率与可迁移性。
source: ICML-2026-Rejected-Public
selection_source: conference_retrieval
motivation: 现有自进化范式让每个智能体孤立学习，冗余挖掘有限经验，导致技能难以泛化。
method: 提出AutoSkills，通过多层技能设计、迭代技能精炼等自动流水线预构建即插即用技能库。
result: 将原始轨迹蒸馏为策略、功能与原子三级技能，实现可迁移的技能复用。
conclusion: 打破孤立学习循环，提升智能体技能获取效率与泛化能力。
---

## Abstract
Learning from experience is crucial for creating more capable LLM-based agents. However, the prevailing self-evolving paradigm is fundamentally inefficient: it forces each agent to learn in isolation, redundantly mining experiences from its own limited capabilities and scarce training data, resulting in expertise that fails to generalize.
To break this cycle, we introduce AutoSkills, a framework that autonomously pre-builds a plug-and-play skill library. AutoSkills operates through a fully automated pipeline built on three synergistic innovations: **i) Multi-Level Skills Design**, which distills raw trajectories into three-tiered hierarchy of strategic plans, functional skills, and atomic skills; **ii) Iterative Skills Refinement**, which automatically revises skills based on execution feedback to continuously improve library quality; and **iii) Exploratory Skill Expansion**, which proactively generates and validates novel skills to expand coverage beyond seed training data.
Using this framework, we construct a reliable plug-and-play skill library using a state-of-the-art agent, GLM-4.6.
We conduct extensive experiments on challenging long-horizon, user-interactive benchmarks, including AppWorld, BFCL-v3, and $\tau^2$-Bench, demonstrating the effectiveness of AutoSkills. 
We also provide strategic insights into how experience transfer impacts model performance.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自主构建即插即用技能库。

### 2. 核心内容
现有自进化范式迫使每个智能体孤立学习，冗余挖掘自身有限经验，导致技能难以泛化。AutoSkills提出全自动流水线，通过多层技能设计、迭代技能精炼等机制预构建即插即用的技能库，将原始轨迹蒸馏为策略、功能与原子三级技能。该框架打破孤立学习循环，显著提升智能体技能获取的效率与可迁移性。

### 3. 对应检索需求
agents capable of self-improvement and autonomous skill acquisition。

### 4. 来源与原文
- Source：ICML-2026-Rejected-Public
- OpenReview：[https://openreview.net/forum?id=rJS7Z3Oaw1](https://openreview.net/forum?id=rJS7Z3Oaw1)
