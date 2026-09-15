---
title: "MemEvolve: Meta-Evolution of Agent Memory Systems"
title_zh: MemEvolve：智能体记忆系统的元进化
authors: "Guibin Zhang, Haotian Ren, Chong Zhan, Junhao Wang, He Zhu, Wangchunshu Zhou, Shuicheng YAN"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/1e41a1afd50901e4fabd439045aa390f5d0448f8.pdf"
tags: ["query:self-evolve"]
score: 9.0
evidence: 元进化框架同时进化智能体经验知识与记忆架构
tldr: 自我进化记忆系统正重塑LLM智能体的进化范式，但现有方法依赖人工设计的记忆架构，其本身静态、无法随任务元适应，限制了智能体进化。作者提出MemEvolve元进化框架，联合进化智能体的经验知识与记忆架构，使系统不仅能积累经验还能元适应不同任务情境。实验表明该框架提升了智能体的跨任务进化与适应能力，推动了自进化智能体架构层面的发展。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有自进化记忆依赖人工静态架构，无法元适应多样任务，限制智能体进化。
method: 提出元进化框架，联合进化智能体的经验知识与记忆架构本身。
result: 使智能体在积累经验的同时能元适应不同任务情境，提升进化能力。
conclusion: 将自进化从经验层推进到记忆架构层，拓展了自进化智能体范式。
---

## Abstract
Self-evolving memory systems are rapidly reshaping the evolutionary paradigm of large language model (LLM)-based agents. Prior work has predominantly relied on manually engineered memory architectures to store trajectories, distill experience, and synthesize reusable tools, enabling agents to evolve on the fly within environment interactions. However, this paradigm is fundamentally constrained by the \textit{staticity} of the memory system itself: while memory facilitates agent-level evolving, the underlying memory architecture cannot be meta-adapted to diverse task contexts. To address this gap, we propose MemEvolve, a meta-evolutionary framework that jointly evolves agents’ experiential knowledge and their memory architecture, allowing agent systems not only to accumulate experience but also to progressively refine how they learn from it. To ground MemEvolve in prior work and promote openness in future self-evolving systems, we introduce EvolveLab, a unified memory codebase that distills twelve representative memory systems into a modular design space (\textit{encode}, \textit{store}, \textit{retrieve}, \textit{manage}), providing a standardized implementation substrate and a fair experimental arena. Extensive evaluations on four challenging agentic benchmarks show that MemEvolve delivers (i) substantial performance gains, improving frameworks such as SmolAgent and Flash-Searcher by up to $17.06\%$, and (ii) strong cross-task and cross-LLM generalization, yielding memory architectures that transfer effectively across diverse benchmarks and backbones.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
元进化框架同时进化智能体经验知识与记忆架构。

### 2. 核心内容
自我进化记忆系统正重塑LLM智能体的进化范式，但现有方法依赖人工设计的记忆架构，其本身静态、无法随任务元适应，限制了智能体进化。作者提出MemEvolve元进化框架，联合进化智能体的经验知识与记忆架构，使系统不仅能积累经验还能元适应不同任务情境。实验表明该框架提升了智能体的跨任务进化与适应能力，推动了自进化智能体架构层面的发展。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=qpkG0eKx4v](https://openreview.net/forum?id=qpkG0eKx4v)
