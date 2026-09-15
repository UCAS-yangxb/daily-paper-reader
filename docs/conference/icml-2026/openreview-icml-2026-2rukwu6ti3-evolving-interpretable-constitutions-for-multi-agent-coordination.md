---
title: Evolving Interpretable Constitutions for Multi-Agent Coordination
title_zh: 为多智能体协调进化可解释宪法
authors: "Ujwal Kumar, Alice Saito, Hershraj Niranjani, Rayan Yessou, Phan Xuan Tan"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f8b674b7ffb663ce9de76481f6fc631b88495f79.pdf"
tags: ["query:self-evolve"]
score: 5.0
evidence: 进化式宪法自动发现多智能体行为规范
tldr: 宪法式AI多关注单模型对齐且使用固定原则，而多智能体系统因涌现的社会动态带来新的对齐挑战。本文提出宪法进化框架，在带生存压力的网格世界模拟中自动发现多智能体语言模型的行为规范，并用融合生产力、生存与冲突的社会稳定度指标量化个体与集体福祉的张力。实验显示对抗性宪法导致社会崩溃，模糊的亲社会原则协调不一致，为多智能体规范的自演化提供研究。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多智能体系统因涌现社会动态带来新对齐挑战，固定原则难以适用。
method: 提出宪法进化框架，在生存压力网格世界中自动发现多智能体行为规范。
result: 对抗性宪法导致社会崩溃，模糊亲社会原则协调不一致。
conclusion: 为多智能体系统中行为规范的自演化与对齐提供新框架。
---

## Abstract
Constitutional AI has focused on single-model alignment using fixed principles. However, multi-agent systems create novel alignment challenges through emergent social dynamics. We present Constitutional Evolution, a framework for automatically discovering behavioral norms in multi-agent LLM systems. Using a grid-world simulation with survival pressure, we study the tension between individual and collective welfare, quantified via a Societal Stability Score $\mathcal{S} \in [0,1]$ that combines productivity, survival, and conflict metrics. Adversarial constitutions lead to societal collapse ($\mathcal{S}=0$), while vague prosocial principles (''be helpful, harmless, honest'') produce inconsistent coordination ($\mathcal{S}=0.249$). Even constitutions designed by Claude 4.5 Opus with explicit knowledge of the objective achieve only moderate performance ($\mathcal{S}=0.332$). Using LLM-driven genetic programming with multi-island evolution, we evolve constitutions maximizing social welfare without explicit guidance toward cooperation. The evolved constitution $\mathcal{C}^*$ achieves 
$\mathcal{S}=0.556\pm0.008$ (123\% higher than human-designed baselines, $N=10$), eliminates conflict, and discovers that minimizing communication (0.9\% vs 62.2\% social actions) outperforms verbose coordination. Our interpretable 
rules demonstrate that cooperative norms can be discovered rather than prescribed.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
进化式宪法自动发现多智能体行为规范。

### 2. 核心内容
宪法式AI多关注单模型对齐且使用固定原则，而多智能体系统因涌现的社会动态带来新的对齐挑战。本文提出宪法进化框架，在带生存压力的网格世界模拟中自动发现多智能体语言模型的行为规范，并用融合生产力、生存与冲突的社会稳定度指标量化个体与集体福祉的张力。实验显示对抗性宪法导致社会崩溃，模糊的亲社会原则协调不一致，为多智能体规范的自演化提供研究。

### 3. 对应检索需求
evolutionary algorithms for evolving agent behaviors and architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=2rukwU6tI3](https://openreview.net/forum?id=2rukwU6tI3)
