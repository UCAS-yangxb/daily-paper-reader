---
title: "Lifting Traces to Logic: Programmatic Skill Induction with Neuro-Symbolic Learning for Long-Horizon Agentic Tasks"
title_zh: 从轨迹到逻辑：面向长程智能体任务的神经符号程序化技能归纳
authors: "Jie-Jing Shao, Haiyan Yin, Yueming Lyu, Xingrui Yu, Lan-Zhe Guo, Ivor Tsang, James Kwok, Yu-Feng Li"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/5f23988a622ad726ee60add79d3a84b1d841e729.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 神经符号技能归纳使智能体从轨迹中自主获取可复用技能
tldr: 针对基础模型智能体长程规划中纯提示推理易失效、既有技能归纳方法无法捕捉条件逻辑的问题，本文提出神经符号技能归纳框架NSI。该方法将交互轨迹提升为模块化、逻辑奠基的程序，通过合成显式控制流与动态变量绑定，让智能体学会在何时为何行动。实验显示该方法支持少样本技能归纳与高效泛化。这为智能体自主获取可复用技能提供了新范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有技能归纳方法生成的状态盲脚本无法捕捉动态环境所需的条件逻辑。
method: 提出神经符号技能归纳NSI，将交互轨迹提升为带控制流和变量绑定的模块化程序。
result: 该方法支持少样本技能归纳，使智能体在动态环境中实现高效泛化。
conclusion: 逻辑奠基的程序化技能为智能体自主技能获取提供了可复用范式。
---

## Abstract
Foundation model-driven agents often struggle with long-horizon planning due to the transient nature of purely prompting-based reasoning. While existing skill induction methods mitigate this by distilling experience into state-blind parameterized scripts, they fail to capture the conditional logic required for robust execution in dynamic environments. In this paper, we propose Neuro-Symbolic Skill Induction (NSI), a framework that lifts interaction traces into modular, logic-grounded programs. By synthesizing explicit control flows and dynamic variable binding, NSI empowers agents to discover when and why to act. This paradigm enables the efficient generalization, allowing agents to induce skills from few-shot examples and flexibly adapt to unseen goals. Experiments on a series of agentic tasks demonstrate that NSI consistently outperforms state-of-the-art baselines, empowering agents to self-evolve into architects of logic-grounded skills. Project Page: https://sh-jj.github.io/NSI.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
神经符号技能归纳使智能体从轨迹中自主获取可复用技能。

### 2. 核心内容
针对基础模型智能体长程规划中纯提示推理易失效、既有技能归纳方法无法捕捉条件逻辑的问题，本文提出神经符号技能归纳框架NSI。该方法将交互轨迹提升为模块化、逻辑奠基的程序，通过合成显式控制流与动态变量绑定，让智能体学会在何时为何行动。实验显示该方法支持少样本技能归纳与高效泛化。这为智能体自主获取可复用技能提供了新范式。

### 3. 对应检索需求
agents capable of self-improvement and autonomous skill acquisition。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=D0Dg8ISjq0](https://openreview.net/forum?id=D0Dg8ISjq0)
