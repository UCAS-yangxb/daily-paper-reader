---
title: "Skill-Pro: Learning Reusable Skills from Experience via Non-Parametric PPO for LLM Agents"
title_zh: Skill-Pro：通过非参数PPO从经验中学习可复用技能的LLM智能体
authors: "Qirui Mi, Zhijian Ma, Mengyue Yang, Haoxuan Li, Yisen Wang, Haifeng Zhang, Jun Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/1bccdd13cafb0f585fe10ee4bc4fb18649e4c959.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 自主从经验学习可复用技能
tldr: 大模型智能体擅长序列决策，却依赖即时推理，在重复场景中反复推导解决方案，导致计算冗余与不稳定。本文提出Skill-Pro，形式化Skill-MDP，通过非参数PPO利用语义梯度从交互经验中自主学习可复用技能。无需参数更新即可将情节叙事转为可执行技能，提升经验复用与技能获取稳定性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM智能体依赖即时推理，重复场景下重复推导，经验复用不足。
method: 提出Skill-Pro，形式化Skill-MDP，以非参数PPO从交互经验中自主学习可复用技能。
result: 将情节叙事转为可执行技能，无需参数更新即可可靠复用。
conclusion: 提升智能体经验复用与技能获取的稳定性。
---

## Abstract
LLM-driven agents excel at sequential decision-making but often rely on on-the-fly reasoning, re-deriving solutions even in recurring scenarios. This insufficient experience reuse leads to computational redundancy and instability. To bridge this gap, we propose **Skill-Pro**, a framework enabling agents to autonomously learn reusable procedural skills from interaction experiences without parameter updates. By formalizing a **Skill-MDP**, Skill-Pro transforms passive episodic narratives into executable Skills defined by activation, execution, and termination conditions to ensure executability. 
To achieve reliable reusability without capability degradation, we introduce **Non-Parametric PPO**, which leverages semantic gradients for high-quality candidate generation and a PPO Gate for robust Skill verification. Through score-based maintenance, Skill-Pro sustains compact, high-quality procedural memory.
Experimental results across in-domain, cross-task, and cross-agent scenarios demonstrate that Skill-Pro achieves superior reuse rates and significant gains with extreme memory compression. Visualized evolutionary trajectories and Skill distributions further reveal how Skill-Pro transparently accumulates, refines, and reuses procedural knowledge to facilitate long-term autonomy.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自主从经验学习可复用技能。

### 2. 核心内容
大模型智能体擅长序列决策，却依赖即时推理，在重复场景中反复推导解决方案，导致计算冗余与不稳定。本文提出Skill-Pro，形式化Skill-MDP，通过非参数PPO利用语义梯度从交互经验中自主学习可复用技能。无需参数更新即可将情节叙事转为可执行技能，提升经验复用与技能获取稳定性。

### 3. 对应检索需求
agents capable of self-improvement and autonomous skill acquisition。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=9kJQjx2B80](https://openreview.net/forum?id=9kJQjx2B80)
