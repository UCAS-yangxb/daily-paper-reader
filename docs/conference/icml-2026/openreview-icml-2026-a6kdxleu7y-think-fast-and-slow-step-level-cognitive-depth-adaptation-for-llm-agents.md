---
title: "Think Fast and Slow: Step-Level Cognitive Depth Adaptation for LLM Agents"
title_zh: 快思考与慢思考：面向LLM智能体的步级认知深度自适应
authors: "Ruihan Yang, Fanghua Ye, Xiang Wei, Ruoqing Zhao, Kang Luo, Xinbo Xu, Bo Zhao, Ruotian Ma, Shanyi Wang, Zhaopeng Tu, Xiaolong Li, Deqing Yang, Liefeng Bo"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/aa891a38c3c128f587073fb41820ac72547169c8.pdf"
tags: ["query:self-evolve"]
score: 4.0
evidence: 逐步动态调整认知深度，是面向LLM智能体的自适应机制
tldr: 针对当前LLM智能体采用固定认知模式、长程任务中步级认知需求差异被忽视而导致低效的问题，本文提出CogRouter框架。该方法基于ACT-R理论设计从本能反应到战略规划的四级认知层次，并通过两阶段训练让智能体在每步动态调整认知深度。实验表明该自适应机制能提升长程任务中的决策效率。这为智能体的自适应行为调节提供了新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有LLM智能体采用固定认知模式，难以适应长程任务中步级变化的认知需求。
method: 提出CogRouter，基于ACT-R设计四级认知层次并用两阶段训练动态调整认知深度。
result: 智能体可在每步自适应选择认知深度，提升长程任务的执行效率。
conclusion: 步级认知深度自适应为智能体动态环境下的高效决策提供了机制。
---

## Abstract
Large language models (LLMs) are increasingly deployed as autonomous agents for multi-turn decision-making tasks. However, current agents typically rely on fixed cognitive patterns: non-thinking models generate immediate responses, while thinking models engage in deep reasoning uniformly. This rigidity is inefficient for long-horizon tasks, where cognitive demands vary significantly from step to step, with some requiring strategic planning and others only routine execution. In this paper, we introduce CogRouter, a framework that trains agents to dynamically adapt cognitive depth at each step. Grounded in ACT-R theory, we design four hierarchical cognitive levels ranging from instinctive responses to strategic planning. Our two-stage training approach includes Cognition-aware Supervised Fine-tuning (CogSFT) to instill stable level-specific patterns, and Cognition-aware Policy Optimization (CoPO) for step-level credit assignment via confidence-aware advantage reweighting. The key insight is that appropriate cognitive depth should maximize the confidence of the resulting action. Experiments on ALFWorld and ScienceWorld demonstrate that CogRouter achieves state-of-the-art performance with superior efficiency.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
逐步动态调整认知深度，是面向LLM智能体的自适应机制。

### 2. 核心内容
针对当前LLM智能体采用固定认知模式、长程任务中步级认知需求差异被忽视而导致低效的问题，本文提出CogRouter框架。该方法基于ACT-R理论设计从本能反应到战略规划的四级认知层次，并通过两阶段训练让智能体在每步动态调整认知深度。实验表明该自适应机制能提升长程任务中的决策效率。这为智能体的自适应行为调节提供了新思路。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=a6KDxLeU7y](https://openreview.net/forum?id=a6KDxLeU7y)
