---
title: "Just-In-Time Reinforcement Learning: Continual Learning in LLM Agents Without Gradient Updates"
title_zh: 即时强化学习：无需梯度更新的LLM智能体持续学习
authors: "Yibo Li, Zijie Lin, Ailin Deng, Xuan Zhang, Yufei He, Shuo Ji, Tri Cao, Bryan Hooi"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d3fd303ad091873ad8b58e9b69e647e715cdc721.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 免训练的持续学习与测试时自适应
tldr: 针对LLM智能体部署后权重冻结、难以持续适应，而传统强化学习成本高且易灾难性遗忘的问题，本文提出即时强化学习框架JitRL。该框架无需梯度更新，维护动态非参数化经验记忆，实时检索相关轨迹估计动作优势，并直接调节LLM输出logits。理论证明该加性调节有效，实验表明其能在测试时持续优化策略，为智能体的持续自适应提供了低成本、无遗忘的解决方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM智能体部署后权重冻结难以持续适应，传统强化学习成本高且易遗忘。
method: 提出JitRL，用动态非参数记忆实时估计优势并直接调节输出logits，无需梯度更新。
result: 理论证明加性调节有效，实验表明可在测试时持续优化策略。
conclusion: 为LLM智能体的持续自适应提供了免训练、低遗忘风险的解决方案。
---

## Abstract
While Large Language Model (LLM) agents excel at general tasks, they inherently struggle with continual adaptation due to the frozen weights after deployment. Conventional reinforcement learning (RL) offers a solution but incurs prohibitive computational costs and the risk of catastrophic forgetting. 
    We introduce Just-In-Time Reinforcement Learning (JitRL), a training-free framework that enables test-time policy optimization without any gradient updates. 
    JitRL maintains a dynamic, non-parametric memory of experiences and retrieves relevant trajectories to estimate action advantages on-the-fly. 
    These estimates are then used to directly modulate the LLM's output logits. 
    We theoretically prove that this additive update rule is the exact closed-form solution to the KL-constrained policy optimization objective. 
    Extensive experiments on WebArena and Jericho demonstrate that JitRL establishes a new state-of-the-art among training-free methods. 
    Crucially, JitRL outperforms the performance of computationally expensive fine-tuning methods (e.g., WebRL) while reducing monetary costs by over 30 times, offering a scalable path for continual learning agents. The code is available at https://github.com/liushiliushi/JitRL.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
免训练的持续学习与测试时自适应。

### 2. 核心内容
针对LLM智能体部署后权重冻结、难以持续适应，而传统强化学习成本高且易灾难性遗忘的问题，本文提出即时强化学习框架JitRL。该框架无需梯度更新，维护动态非参数化经验记忆，实时检索相关轨迹估计动作优势，并直接调节LLM输出logits。理论证明该加性调节有效，实验表明其能在测试时持续优化策略，为智能体的持续自适应提供了低成本、无遗忘的解决方案。

### 3. 对应检索需求
lifelong learning and continual adaptation in artificial agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=pLvye0zHUC](https://openreview.net/forum?id=pLvye0zHUC)
