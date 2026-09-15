---
title: "$\\texttt{Multi}^2$: Hierarchical Multi-Agent Decision-Making with LLM-Based Agents in Interactive Environments"
title_zh: Multi2：交互环境中基于LLM智能体的分层多智能体决策
authors: "Sangeun Park, Minhae Kwon"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/8ee1247f66c76f12dd99c3970859a2f45f7ed70a.pdf"
tags: ["query:self-evolve"]
score: 5.0
evidence: 智能体在动态交互环境中规划、行动与适应
tldr: LLM智能体在长程交互中常出现目标漂移，规划与行动不稳定，难以在动态环境中持续适应。作者提出Multi2分层多智能体决策框架，将智能体行为分解为互补角色：高层智能体经监督微调生成情境化子目标，低层智能体负责执行。该设计缓解了目标漂移问题，提升了在交互式环境中的长程决策与适应能力。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM智能体长程决策脆弱，易出现目标漂移，难以在动态环境中持续适应。
method: 提出分层多智能体框架，将行为分解为高层子目标生成与低层执行两种角色。
result: 该框架缓解目标漂移，提升了交互环境中的长程决策稳定性。
conclusion: 表明分层角色分解可增强智能体在动态环境中的适应能力。
---

## Abstract
A central goal of large language model (LLM) research is to build agentic systems that can plan, act, and adapt through sustained interaction with dynamic environments. While recent LLM-based agents exhibit impressive contextual reasoning, their long-horizon decision-making remains fragile, often suffering from $\textit{objective drift}$, where goals and plans drift over extended interactions.
We introduce $\texttt{Multi}^2$, a hierarchical multi-agent decision-making framework that explicitly decomposes agent behavior into complementary roles. A high-level agent ($\texttt{System 1}$) focuses on context-aware sub-goal generation using supervised fine-tuning (SFT), while a low-level agent ($\texttt{System 2}$) executes atomic actions through offline-to-online reinforcement learning (RL) in interactive environments. This separation enables stable long-horizon control, mitigates objective drift, and allows efficient adaptation.
Across diverse interactive environments, $\texttt{Multi}^2$ consistently outperforms strong agentic baselines, demonstrating improved robustness and coordination in multi-turn interaction. Beyond performance, we introduce and release three hierarchical benchmark datasets, filling a long-standing gap in training and evaluating hierarchical decision-making for LLM-based agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
智能体在动态交互环境中规划、行动与适应。

### 2. 核心内容
LLM智能体在长程交互中常出现目标漂移，规划与行动不稳定，难以在动态环境中持续适应。作者提出Multi2分层多智能体决策框架，将智能体行为分解为互补角色：高层智能体经监督微调生成情境化子目标，低层智能体负责执行。该设计缓解了目标漂移问题，提升了在交互式环境中的长程决策与适应能力。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=H0tMEp0ZmO](https://openreview.net/forum?id=H0tMEp0ZmO)
