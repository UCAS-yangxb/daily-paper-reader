---
title: "EvoMAS: Evolutionary Generation of Multi-Agent Systems"
title_zh: EvoMAS：多智能体系统的进化式生成
authors: "Yuntong Hu, Yuting Zhang, Matthew Trager, Yi Zhang, Shuo Yang, Wei Xia, Stefano Soatto"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/410b88190222509514e11e3aeed3145745decae0.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 在配置空间通过反馈驱动变异与交叉进化生成多智能体系统
tldr: 针对LLM多智能体系统架构设计依赖人工、脆弱且难以泛化，以及现有自动生成方法存在可执行性差或模板僵化的问题，本文提出EvoMAS。该方法将多智能体系统生成建模为结构化配置生成，在配置空间中执行进化搜索，并采用反馈驱动的变异与交叉操作。实验表明该框架在提升表达能力和适应性的同时改善了架构生成质量。这为智能体架构的自动化进化设计提供了新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有多智能体系统架构设计费时脆弱，自动生成方法受限于代码生成或僵化模板。
method: 提出EvoMAS，将多智能体系统生成建模为配置生成，在配置空间进行反馈驱动变异与交叉。
result: 该方法在提升架构表达力与适应性的同时改善了自动生成系统的鲁棒性。
conclusion: 进化式配置生成可自动化地设计更具泛化能力的多智能体系统架构。
---

## Abstract
Large language model (LLM)-based multi-agent systems (MAS) show strong promise for complex reasoning, planning, and tool-augmented tasks, but designing effective MAS architectures remains labor-intensive, brittle, and hard to generalize. Existing automatic MAS generation methods either rely on code generation, which often leads to executability and robustness failures, or impose rigid architectural templates that limit expressiveness and adaptability. We propose Evolutionary Generation of Multi-Agent Systems (EvoMAS), which formulates MAS generation as structured configuration generation. EvoMAS performs evolutionary generation in configuration space. Specifically, EvoMAS selects initial configurations from a pool, applies feedback-conditioned mutation and crossover guided by execution traces, and iteratively refines both the candidate pool and an experience memory. We evaluate EvoMAS on diverse benchmarks, including BBEH, SWE-Bench, and WorkBench, covering reasoning, software engineering, and tool-use tasks. EvoMAS consistently improves task performance over both human-designed MAS and prior automatic MAS generation methods, while producing generated systems with higher executability and runtime robustness. EvoMAS outperforms the agent evolution method EvoAgent by +10.5 points on BBEH reasoning and +7.1 points on WorkBench. With Claude-4.5-Sonnet, EvoMAS also reaches 79.1% on SWE-Bench-Verified, matching the top of the leaderboard. Code is available at https://github.com/amazon-science/EvoMAS

---

## 论文详细总结（自动生成）

### 1. 检索相关性
在配置空间通过反馈驱动变异与交叉进化生成多智能体系统。

### 2. 核心内容
针对LLM多智能体系统架构设计依赖人工、脆弱且难以泛化，以及现有自动生成方法存在可执行性差或模板僵化的问题，本文提出EvoMAS。该方法将多智能体系统生成建模为结构化配置生成，在配置空间中执行进化搜索，并采用反馈驱动的变异与交叉操作。实验表明该框架在提升表达能力和适应性的同时改善了架构生成质量。这为智能体架构的自动化进化设计提供了新思路。

### 3. 对应检索需求
evolutionary algorithms for evolving agent behaviors and architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ic0AGRIkmY](https://openreview.net/forum?id=ic0AGRIkmY)
