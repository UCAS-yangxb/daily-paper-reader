---
title: "AgentConductor: Topology Evolution for Multi-Agent Competition-Level Code Generation"
title_zh: AgentConductor：面向多智能体竞赛级代码生成的拓扑演化
authors: "Siyu Wang, Ruotian Lu, Zhihao Yang, Yuchao Wang, Yanzhou Zhang, Lei Xu, Qimin Xu, Guojun Yin, Cailian Chen, Xinping Guan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/6ffc4b8b771eaf3318c96846c00a057cf5739573.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 通过强化学习演化多智能体拓扑结构
tldr: 现有LLM多智能体系统依赖预定义拓扑，既不能随任务难度调整拓扑密度，也无法在单实例内利用执行反馈进行精炼，导致冗余通信与性能瓶颈。为此作者提出AgentConductor，以基于LLM的编排智能体为核心，用强化学习优化多智能体系统的拓扑演化。实验表明该方法在竞赛级代码生成任务上能自适应拓扑并提升性能，为多智能体协作结构的自动演化提供了新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有多智能体系统拓扑固定，无法按任务难度自适应且缺乏实例内精炼，造成通信冗余。
method: 提出以LLM编排智能体为核心、用强化学习优化拓扑演化的多智能体框架。
result: 在竞赛级代码生成任务上实现拓扑自适应，减少冗余通信并提升协作性能。
conclusion: 表明通过强化学习演化多智能体拓扑可有效提升复杂任务表现。
---

## Abstract
Large language model(LLM)-driven multi-agent systems(MAS) coordinate specialized agents through predefined topologies and show promise for complex tasks such as competition-level code generation. Recent studies demonstrate that carefully designed multi-agent workflows and communication graphs can significantly improve code generation performance by leveraging collaborative reasoning. However, existing methods neither adapt topology density to task difficulty nor refine the topology within an instance using execution feedback, which leads to redundant communication and performance bottlenecks. To address these issues, we propose AgentConductor: a reinforcement learning-optimized MAS with an LLM-based orchestrator agent as its core, which enables end-to-end feedback-driven dynamic generation of interaction topologies. For each query, AgentConductor infers agent roles and task difficulty, then constructs a task-adapted, density-aware layered directed acyclic graph(DAG) topology, underpinned by two key innovations. First, we design a novel topology density function to quantify communication-aware multi-agent interactions. Second, we adopt difficulty interval partitioning to avoid excessive pruning for precise topological density upper bound measurement per difficulty level and finer-grained control. Across five code datasets, AgentConductor outperforms the strongest baseline by up to 14.6\% in pass@1, with 13\% lower topology density and 68\% lower token cost.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
通过强化学习演化多智能体拓扑结构。

### 2. 核心内容
现有LLM多智能体系统依赖预定义拓扑，既不能随任务难度调整拓扑密度，也无法在单实例内利用执行反馈进行精炼，导致冗余通信与性能瓶颈。为此作者提出AgentConductor，以基于LLM的编排智能体为核心，用强化学习优化多智能体系统的拓扑演化。实验表明该方法在竞赛级代码生成任务上能自适应拓扑并提升性能，为多智能体协作结构的自动演化提供了新思路。

### 3. 对应检索需求
evolutionary algorithms for evolving agent behaviors and architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=4bLahBrVBs](https://openreview.net/forum?id=4bLahBrVBs)
