---
title: Continual GUI Agents
title_zh: 持续GUI智能体
authors: "Ziwei Liu, Borui Kang, Hangjie Yuan, Zixiang Zhao, Wei Li, Yifan Zhu, Tao Feng"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/b38a5ea86afbcc10adef11c2f9b34d7fd8ba824c.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: GUI智能体在领域与分辨率漂移下的持续学习
tldr: 数字环境不断变化，新的GUI数据带来新领域或分辨率，使在静态环境训练的智能体性能退化。本文提出持续GUI智能体这一新任务，要求其在领域与分辨率漂移下进行持续学习。作者提出GUI-AiF强化微调框架，通过锚点奖励与锚区奖励两种新奖励稳定持续学习。实验表明该方法能在界面分布持续变化时维持稳定定位，为持续自适应智能体提供新思路。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: GUI环境分布不断变化，静态环境训练的智能体在领域与分辨率漂移下性能退化。
method: 提出GUI-AiF强化微调框架，用锚点奖励与锚区奖励稳定持续学习。
result: 实验显示该方法在界面分布漂移时能维持稳定定位。
conclusion: 为GUI智能体的持续学习与自适应提供新任务与解决方案。
---

## Abstract
As digital environments (data distribution) are in flux, with new GUI data arriving over time-introducing new domains or resolutions-agents trained on static environments deteriorate in performance. In this work, we introduce Continual GUI Agents, a new task that requires GUI agents to perform continual learning under shifted domains and resolutions. We find existing methods fail to maintain stable grounding as GUI distributions shift over time, due to the diversity of UI interaction points and regions in fluxing scenarios. To address this, we introduce GUI-Anchoring in Flux (GUI-AiF), a new reinforcement fine-tuning framework that stabilizes continual learning through two novel rewards: Anchoring Point Reward in Flux (APR-iF) and Anchoring Region Reward in Flux (ARR-iF). These rewards guide the agents to align with shifting interaction points and regions, mitigating the tendency of existing reward strategies to over-adapt to static grounding cues (e.g., fixed coordinates or element scales). Extensive experiments show GUI-AiF surpasses state-of-the-art baselines. Our work establishes the first continual learning framework for GUI agents, revealing the untapped potential of reinforcement fine-tuning for continual GUI Agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
GUI智能体在领域与分辨率漂移下的持续学习。

### 2. 核心内容
数字环境不断变化，新的GUI数据带来新领域或分辨率，使在静态环境训练的智能体性能退化。本文提出持续GUI智能体这一新任务，要求其在领域与分辨率漂移下进行持续学习。作者提出GUI-AiF强化微调框架，通过锚点奖励与锚区奖励两种新奖励稳定持续学习。实验表明该方法能在界面分布持续变化时维持稳定定位，为持续自适应智能体提供新思路。

### 3. 对应检索需求
lifelong learning and continual adaptation in artificial agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=7WeA5TAjHK](https://openreview.net/forum?id=7WeA5TAjHK)
