---
title: Continual Learning through Control Minimization
title_zh: 通过控制最小化实现持续学习
authors: "Sander de Haan, Yassine Taoudi-Benchekroun, Pau Vilimelis Aceituno, Benjamin F Grewe"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/3313191f676007297de14b78bafe42ec4e8fd8c4.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 将持续学习重构为控制问题以缓解遗忘
tldr: 灾难性遗忘是神经网络顺序学习任务时的根本难题。本文将持续学习重构为控制问题，让学习信号与保持信号在神经活动动态中相互竞争，把正则惩罚转化为保护先前任务表征的保持信号。学习通过最小化整合新任务所需的控制努力进行，在平衡点处权重更新隐式编码了完整的先前任务曲率，称为持续自然梯度，无需显式存储曲率。实验验证了该框架，为持续学习提供新视角。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 灾难性遗忘是神经网络顺序学习任务时的根本难题。
method: 将持续学习重构为控制问题，用学习与保持信号竞争，导出持续自然梯度。
result: 在平衡点隐式编码先前任务曲率，无需显式存储，实验验证有效。
conclusion: 为持续学习提供了控制论视角的新框架。
---

## Abstract
Catastrophic forgetting remains a fundamental challenge for neural networks when tasks are trained sequentially. In this work, we reformulate continual learning as a control problem where learning and preservation signals compete within neural activity dynamics. We convert regularization penalties into preservation signals that protect prior-task representations. Learning then proceeds by minimizing the control effort required to integrate new tasks while competing with the preservation of prior tasks. At equilibrium, the neural activities produce weight updates that implicitly encode the full prior-task curvature, a property we term the *continual-natural gradient*, requiring no explicit curvature storage. Experiments confirm that our learning framework recovers true prior-task curvature and enables task discrimination, outperforming existing methods on standard benchmarks without replay.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
将持续学习重构为控制问题以缓解遗忘。

### 2. 核心内容
灾难性遗忘是神经网络顺序学习任务时的根本难题。本文将持续学习重构为控制问题，让学习信号与保持信号在神经活动动态中相互竞争，把正则惩罚转化为保护先前任务表征的保持信号。学习通过最小化整合新任务所需的控制努力进行，在平衡点处权重更新隐式编码了完整的先前任务曲率，称为持续自然梯度，无需显式存储曲率。实验验证了该框架，为持续学习提供新视角。

### 3. 对应检索需求
methods for lifelong learning and continual adaptation in autonomous intelligent agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ix1HdZkO8U](https://openreview.net/forum?id=ix1HdZkO8U)
