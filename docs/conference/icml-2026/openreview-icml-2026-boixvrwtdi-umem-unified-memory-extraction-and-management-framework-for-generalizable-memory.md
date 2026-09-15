---
title: "UMEM: Unified Memory Extraction and Management Framework for Generalizable Memory"
title_zh: UMEM：面向可泛化记忆的统一记忆提取与管理框架
authors: "Yongshi Ye, Hui Jiang, Feihu Jiang, Tian Lan, Yichao Du, Biao Fu, Xiaodong Shi, Qianghuai Jia, Longyue Wang, Weihua Luo"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9bcba03fc57063491f6d3b408af5094d4d663f30.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 自进化大模型智能体记忆框架
tldr: 自进化记忆被视为大语言模型智能体的可训练参数，但现有方法主要优化记忆管理，将记忆提取当作静态过程，导致智能体积累实例噪声而泛化不佳。作者提出UMEM统一记忆提取与管理框架，联合优化同一个LLM同时完成经验提炼与记忆库更新，并引入语义邻域建模以缓解过拟合。实验显示该方法能获得更稳健、更可泛化的记忆。该工作推动了LLM智能体自进化记忆的统一优化。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自进化记忆作为LLM智能体的可训练参数，但现有方法只优化记忆管理，将提取视为静态过程，导致泛化差。
method: 提出UMEM自进化智能体框架，联合优化LLM同时进行记忆提取与管理，并引入语义邻域建模缓解过拟合。
result: 减少了对具体实例的过拟合，提升了记忆的泛化能力。
conclusion: 为LLM智能体的自进化记忆提供了统一优化方案。
---

## Abstract
Self-evolving memory serves as the trainable parameters for Large Language Models (LLMs)-based agents, where extraction (distilling insights from experience) and management (updating the memory bank) must be tightly coordinated. 
Existing methods predominantly optimize memory management while treating memory extraction as a static process, resulting in poor generalization, where agents accumulate instance-specific noise rather than robust memories.
To address this, we propose Unified Memory Extraction and Management (UMEM), a self-evolving agent framework that jointly optimizes a LLM to simultaneously extract and manage memories.
To mitigate overfitting to specific instances, we introduce Semantic Neighborhood Modeling and optimize the model with a neighborhood-level marginal utility reward via GRPO.
This approach ensures memory generalizability by evaluating memory utility across clusters of semantically related queries.
Extensive experiments across five benchmarks demonstrate that UMEM significantly outperforms highly competitive baselines, achieving up to 11.49 points improvement in multi-turn interactive tasks. Furthermore, UMEM maintains a stable improvement trend during continuous evolution.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自进化大模型智能体记忆框架。

### 2. 核心内容
自进化记忆被视为大语言模型智能体的可训练参数，但现有方法主要优化记忆管理，将记忆提取当作静态过程，导致智能体积累实例噪声而泛化不佳。作者提出UMEM统一记忆提取与管理框架，联合优化同一个LLM同时完成经验提炼与记忆库更新，并引入语义邻域建模以缓解过拟合。实验显示该方法能获得更稳健、更可泛化的记忆。该工作推动了LLM智能体自进化记忆的统一优化。

### 3. 对应检索需求
large language model based agents with self-evolution capabilities。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=BoiXvrwtdi](https://openreview.net/forum?id=BoiXvrwtdi)
