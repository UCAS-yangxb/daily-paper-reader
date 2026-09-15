---
title: "PathWise: Planning through World Model for Automated Heuristic Design via Self-Evolving LLMs"
title_zh: PathWise：通过世界模型规划、由自进化大模型驱动的自动启发式设计
authors: "Oguzhan Gungordu, Siheng Xiong, Faramarz Fekri"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/faa9536e47383d2283c1ccdef674c8feed96f577.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 通过世界模型规划的自进化大模型启发式设计
tldr: 针对自动启发式设计依赖固定进化规则与静态提示模板、导致生成短视与评估冗余的问题，本文提出多智能体推理框架PathWise。该方法把启发式生成建模为在蕴含图上的序贯决策过程，将蕴含图作为搜索轨迹的紧凑有状态记忆，使系统能携带并复用历史决策。实验表明该框架能进行更有远见的启发式设计，为组合优化中的自进化LLM启发式生成提供了新范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自动启发式设计依赖固定进化规则与静态提示，导致生成短视与冗余评估。
method: 提出PathWise，将启发式生成建模为蕴含图上的序贯决策并复用历史决策。
result: 系统能进行更具远见的启发式设计，减少冗余评估并提升推理质量。
conclusion: 为组合优化中自进化LLM驱动的自动启发式设计提供了新范式。
---

## Abstract
Large Language Models (LLMs) have enabled automated heuristic design (AHD) for combinatorial optimization problems (COPs), but existing frameworks' reliance on fixed evolutionary rules and static prompt templates often leads to myopic heuristic generation, redundant evaluations, and limited reasoning about how new heuristics should be derived. We propose a novel multi-agent reasoning framework, referred to as Planning through World Model for Automated Heuristic Design via Self-Evolving LLMs (PathWise), which formulates heuristic generation as a sequential decision process over an entailment graph serving as a compact, stateful memory of the search trajectory. This approach allows the system to carry forward past decisions and reuse or avoid derivation information across generations. A policy agent plans evolutionary actions, a world model agent generates heuristic rollouts conditioned on those actions, and critic agents provide routed reflections summarizing lessons from prior steps, shifting LLM-based AHD from trial-and-error evolution toward state-aware planning through reasoning. Experiments across diverse COPs show that PathWise converges faster to better heuristics, generalizes across different LLM backbones, and scales to larger problem sizes.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过世界模型规划的自进化大模型启发式设计。

### 2. 核心内容
针对自动启发式设计依赖固定进化规则与静态提示模板、导致生成短视与评估冗余的问题，本文提出多智能体推理框架PathWise。该方法把启发式生成建模为在蕴含图上的序贯决策过程，将蕴含图作为搜索轨迹的紧凑有状态记忆，使系统能携带并复用历史决策。实验表明该框架能进行更有远见的启发式设计，为组合优化中的自进化LLM启发式生成提供了新范式。

### 3. 对应检索需求
large language model based agents with self-evolution capabilities。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=aiOv6NhF3N](https://openreview.net/forum?id=aiOv6NhF3N)
