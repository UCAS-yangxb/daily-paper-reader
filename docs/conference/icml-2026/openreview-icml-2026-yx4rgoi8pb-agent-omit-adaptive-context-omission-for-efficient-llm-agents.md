---
title: "Agent-Omit: Adaptive Context Omission for Efficient LLM Agents"
title_zh: Agent-Omit：面向高效LLM智能体的自适应上下文省略
authors: "Yansong Ning, Jun Fang, Naiqiang Tan, Hao Liu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d8764dda45a3b97087d4f031004ed740769493ec.pdf"
tags: ["query:self-evolve"]
score: 4.0
evidence: LLM智能体自适应省略冗余思考与观察
tldr: 多轮智能体交互中，现有方法平等对待整条轨迹，忽视了各轮思考必要性与观察效用差异，导致上下文冗余。作者先量化分析思考与观察对智能体效能和效率的影响，进而提出Agent-Omit统一训练框架，使LLM智能体自适应省略冗余思考与观察。实验显示该方法在保持效能的同时提升了智能体运行效率，为自适应上下文管理提供了方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有方法平等对待交互轨迹，忽视各轮思考与观察效用差异造成冗余。
method: 提出统一训练框架，让LLM智能体自适应省略冗余的思考与观察内容。
result: 在保持效能的同时提升多轮交互效率，验证了自适应省略的有效性。
conclusion: 为智能体上下文的自适应管理提供了可复用训练方法。
---

## Abstract
Managing agent context (e.g., thought and observation) during multi-turn
agent-environment interactions is an emerging strategy to improve agent efficiency. 
However, existing studies treat the entire interaction trajectories equally, overlooking the thought necessity and observation utility varies across turns.
To this end, we first conduct quantitative investigations into how thought and observation affect agent effectiveness and efficiency.
Based on our findings, we propose Agent-Omit, a unified training framework that empowers LLM agents to adaptively omit redundant thoughts and observations.
Specifically, we first synthesize a small amount of cold-start data, including both single-turn and multi-turn omission scenarios, to fine-tune the agent for omission behaviors. 
Furthermore, we introduce an omit-aware agentic reinforcement learning approach, incorporating a dual sampling mechanism and a tailored omission reward to incentivize the agent's adaptive omission capability.
Theoretically, we prove that the deviation of our omission policy is upper-bounded by KL-divergence.
Experimental results on five agent benchmarks show that our constructed Agent-Omit-8B could obtain performance comparable to seven frontier LLM agent, and achieve the best effectiveness-efficiency trade-off than seven efficient LLM agents methods.
Our code and data are avaliable at https://github.com/usail-hkust/Agent-Omit.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
LLM智能体自适应省略冗余思考与观察。

### 2. 核心内容
多轮智能体交互中，现有方法平等对待整条轨迹，忽视了各轮思考必要性与观察效用差异，导致上下文冗余。作者先量化分析思考与观察对智能体效能和效率的影响，进而提出Agent-Omit统一训练框架，使LLM智能体自适应省略冗余思考与观察。实验显示该方法在保持效能的同时提升了智能体运行效率，为自适应上下文管理提供了方案。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=YX4rgoI8pB](https://openreview.net/forum?id=YX4rgoI8pB)
