---
title: "CATArena: Evaluating Evolutionary Capabilities of Code Agents via Iterative Tournaments"
title_zh: CATArena：通过迭代锦标赛评估代码智能体的进化能力
authors: "Lingyue Fu, Xin Ding, Linyue Pan, Yaoming Zhu, Shao Zhang, Lin Qiu, Xuezhi Cao, Xunliang Cai, Jiaxin Ding, Weiwen Liu, Weinan Zhang, Yong Yu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/b0ecee835bb12ab78de71038956558f31bb6af07.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 通过迭代锦标赛评估代码智能体的进化能力
tldr: 当前LLM代码智能体评估多聚焦单轮生成，无法衡量持续代码优化与多轮迭代发展能力。作者提出CATArena框架，让智能体在迭代锦标赛中通过自我反思和同伴学习不断精炼代码，并提出双重指标将静态生成能力与进化潜力解耦。实验揭示智能体进化潜力与静态能力存在差异，为评估自我进化智能体提供了新基准。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有代码智能体评估只关注单轮生成，无法衡量持续优化与进化潜力。
method: 提出迭代锦标赛框架，让智能体经自我反思与同伴学习精炼代码，并用双指标评估。
result: 实验表明智能体进化潜力可与静态生成能力解耦，暴露评估盲区。
conclusion: 为自我进化代码智能体提供了衡量进化能力的新评测范式。
---

## Abstract
Current evaluation for Large Language Model (LLM) code agents predominantly focus on generating functional code in single-turn scenarios, which fails to evaluate the agent's capability for continuous code optimization and multi-turn iterative development. To bridge this gap, we introduce CATArena, a framework designed to evaluate the evolutionary capabilities of code agents via iterative tournaments. Agents engage in multi-turn tournaments and continuously refine their code through self-reflection and peer-learning based on comprehensive execution feedback. For evaluation, we propose a dual-metric system to decouple static generation proficiency from evolutionary potential. Extensive experiments reveal that an agent's evolutionary potential is not strictly correlated with its initial proficiency. Our analysis further reveals that current agents struggle to concurrently leverage both peer-learning and self-reflection for effective performance gains. Furthermore, the results validate CATArena's high extensibility and resistance to variance tasks, establishing it as a continuous and reliable standard for assessing the evolutionary capability of LLM code agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过迭代锦标赛评估代码智能体的进化能力。

### 2. 核心内容
当前LLM代码智能体评估多聚焦单轮生成，无法衡量持续代码优化与多轮迭代发展能力。作者提出CATArena框架，让智能体在迭代锦标赛中通过自我反思和同伴学习不断精炼代码，并提出双重指标将静态生成能力与进化潜力解耦。实验揭示智能体进化潜力与静态能力存在差异，为评估自我进化智能体提供了新基准。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=913g1X1YAW](https://openreview.net/forum?id=913g1X1YAW)
