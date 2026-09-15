---
title: "EvoMAS: Heuristics in the Loop—Evolving Smarter Agentic Workflows"
title_zh: EvoMAS：让智能体工作流在循环中进化得更聪明
authors: "Yangbo Wei, Zhen Huang, Ronghao Xu, Hong Wang, WEI W. XING"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/4ff6c6e50e816f674b8d4deed33770f295b6a205.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 仿生进化策略演化智能体工作流与角色
tldr: 构建高效多智能体系统通常需要人工设计，现有自动化方法生成模板化智能体、优化单一且忽视任务复杂度梯度。作者提出EvoMAS仿生进化框架，核心是包含七种进化策略的动态算子库，配合角色级进化精炼智能体专业化与协作模式，以及课程引导的调度。实验表明该框架能自动演化出更优的多智能体工作流，为智能体架构的自进化提供了进化计算方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多智能体系统构建依赖人工设计，现有自动化方法模板化且忽视任务复杂度梯度。
method: 提出含七种进化策略、角色级进化与课程调度的仿生多智能体进化框架。
result: 能自动演化出更高效的智能体工作流与协作模式。
conclusion: 证明进化算法可有效驱动多智能体架构与行为的自动演化。
---

## Abstract
The rapid development of Large Language Models has driven Multi-Agent Systems (MAS) growth, but constructing efficient MAS requires labor-intensive manual design. Current automation methods generate templated agents, use monolithic optimization, and ignore task complexity gradients. This paper presents Evolutionary MAS (EvoMAS), a biologically-inspired framework whose core is a dynamic and diverse repertoire of seven evolutionary strategies---six biologically-inspired operators (3 exploration, 3 exploitation) together with a custom operator for domain-specific transformations---driven by adaptive strategy selection. These are complemented by role-level evolution that refines agent specialization and collaboration patterns, and a curriculum-guided schedule that evolves workflows from simple to complex tasks with cross-stage stability. Additionally, to resolve the contradiction between the inefficiency of pure evolution and the rigidity of manual design, we introduce the *Cyber Creator*, a meta-controller that conducts heuristics-in-the-loop learning by formulating and reflectively updating evolutionary rules and strategies. Evaluations demonstrate that EvoMAS consistently outperforms existing methods across multiple domains while maintaining cost efficiency, with roles evolving from homogeneous actors to specialized reasoning ensembles.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
仿生进化策略演化智能体工作流与角色。

### 2. 核心内容
构建高效多智能体系统通常需要人工设计，现有自动化方法生成模板化智能体、优化单一且忽视任务复杂度梯度。作者提出EvoMAS仿生进化框架，核心是包含七种进化策略的动态算子库，配合角色级进化精炼智能体专业化与协作模式，以及课程引导的调度。实验表明该框架能自动演化出更优的多智能体工作流，为智能体架构的自进化提供了进化计算方案。

### 3. 对应检索需求
evolutionary algorithms for evolving agent behaviors and architectures。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=cdWnpXkcQo](https://openreview.net/forum?id=cdWnpXkcQo)
