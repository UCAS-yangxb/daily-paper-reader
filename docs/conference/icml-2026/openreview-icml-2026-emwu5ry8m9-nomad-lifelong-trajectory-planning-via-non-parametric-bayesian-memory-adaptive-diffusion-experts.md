---
title: "NOMAD: Lifelong Trajectory Planning via Non-Parametric Bayesian Memory-Adaptive Diffusion Experts"
title_zh: NOMAD：基于非参数贝叶斯记忆自适应扩散专家的终身轨迹规划
authors: "Yixian Chen, Rufan Bai, Jiangbin Zheng, Yimin Wang, Tiantian CHEN, Wei Wang, Yuhuan Lu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d1c1fb8aca1386b5f851fe8cd9d097c39695e998.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 终身持续适应且不遗忘
tldr: 自动驾驶在开放环境中需持续适应罕见长尾场景，同时不遗忘已有驾驶技能，但静态模型与规则控制器难以应对不断变化的交通动态。作者提出NOMAD终身轨迹规划框架，将非参数贝叶斯记忆与扩散式轨迹生成结合，把增长的场景上下文映射到动态增长的扩散专家集合。实验表明该方法能在长尾场景中持续适应并避免灾难性遗忘。该工作为终身学习与持续适应提供了记忆自适应的通用思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自动驾驶在开放环境中需持续适应长尾场景，同时避免遗忘已学驾驶技能，现有静态模型与规则控制器难以应对。
method: 提出NOMAD框架，将非参数贝叶斯记忆与扩散式轨迹生成结合，把不断增长的场景上下文映射到动态增长的专家集合。
result: 在长尾场景中实现持续适应且无灾难性遗忘，缓解了稳定性与可塑性之间的权衡。
conclusion: 为终身学习型轨迹规划提供了可扩展的记忆自适应方案。
---

## Abstract
Autonomous vehicles operating in open-world environments must continually adapt to rare long-tail scenarios while preserving previously acquired driving skills. However, existing trajectory planning approaches struggle with this stability--plasticity trade-off, as they rely on static models or rigid rule-based controllers that cannot robustly handle evolving and complex traffic dynamics. Against this background, we propose **NOMAD**, a lifelong trajectory planning framework that integrates non-parametric Bayesian memory with diffusion-based trajectory generation, enabling continuous adaptation to long-tail scenarios without catastrophic forgetting. Our method maps growing scene contexts to a dynamically growing set of discrete memory clusters, which guide a conditional diffusion model to function as a mixture of experts specialized for diverse driving behaviors. To retain past knowledge during incremental learning, we introduce a generative replay mechanism that synthesizes pseudo-experiences from previously learned memory clusters. Extensive closed-loop evaluations on the nuPlan benchmark demonstrate that our approach achieves state-of-the-art performance on long-tail scenarios, improving the interPlan score by **9.4%** over the strongest baseline, while maintaining competitive performance on regular driving benchmarks. Moreover, our method exhibits robust continual learning capability, achieving the highest average closed-loop score with positive backward transfer when adapting to sequentially introduced long-tail scenarios.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
终身持续适应且不遗忘。

### 2. 核心内容
自动驾驶在开放环境中需持续适应罕见长尾场景，同时不遗忘已有驾驶技能，但静态模型与规则控制器难以应对不断变化的交通动态。作者提出NOMAD终身轨迹规划框架，将非参数贝叶斯记忆与扩散式轨迹生成结合，把增长的场景上下文映射到动态增长的扩散专家集合。实验表明该方法能在长尾场景中持续适应并避免灾难性遗忘。该工作为终身学习与持续适应提供了记忆自适应的通用思路。

### 3. 对应检索需求
lifelong learning and continual adaptation in artificial agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=emwU5Ry8M9](https://openreview.net/forum?id=emwU5Ry8M9)
