---
title: "MonoScale: Scaling Multi-Agent System with Monotonic Improvement"
title_zh: MonoScale：以单调改进方式扩展多智能体系统
authors: "Shuai Shao, Yixiang Liu, Bingwei Lu, Weinan Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/097d2bafdd70497480aef1e760dd4cec90d9141d.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 扩展感知框架持续集成新智能体并通过记忆提升路由
tldr: 针对LLM多智能体系统扩展智能体池时路由器冷启动导致性能崩溃的问题，本文提出MonoScale扩展感知更新框架。该方法主动生成智能体条件化的熟悉任务，采集成功与失败交互证据并蒸馏为可审计的自然语言记忆来指导路由。通过将顺序增强建模为上下文老虎机，系统在持续集成新智能体时实现单调性能提升。这为智能体系统的持续扩展与自我改进提供了可行方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多智能体系统扩展智能体池时路由器冷启动易引发性能崩溃。
method: 提出扩展感知更新框架，生成熟悉任务并将交互证据蒸馏为记忆指导路由。
result: 顺序增强被建模为上下文老虎机，使系统扩展时保持单调性能改进。
conclusion: 该方法支持智能体系统在持续集成新成员时稳定提升整体能力。
---

## Abstract
In recent years, LLM-based multi-agent systems (MAS) have advanced rapidly, using a router to decompose tasks and delegate subtasks to specialized agents. A natural way to expand capability is to scale up the agent pool by continually integrating new functional agents or tool interfaces, but naive expansion can trigger performance collapse when the router cold-starts on newly added, heterogeneous, and unreliable agents. We propose MonoScale, an expansion-aware update framework that proactively generates a small set of agent-conditioned familiarization tasks, harvests evidence from both successful and failed interactions, and distills it into auditable natural-language memory to guide future routing. We formalize sequential augmentation as a contextual bandit and perform trust-region memory updates, yielding a monotonic non-decreasing performance guarantee across onboarding rounds under a non-interfering expansion assumption. Experiments on GAIA and Humanity's Last Exam show stable gains as the agent pool grows, outperforming naive scale-up and strong-router fixed-pool baselines. Our code is available here.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
扩展感知框架持续集成新智能体并通过记忆提升路由。

### 2. 核心内容
针对LLM多智能体系统扩展智能体池时路由器冷启动导致性能崩溃的问题，本文提出MonoScale扩展感知更新框架。该方法主动生成智能体条件化的熟悉任务，采集成功与失败交互证据并蒸馏为可审计的自然语言记忆来指导路由。通过将顺序增强建模为上下文老虎机，系统在持续集成新智能体时实现单调性能提升。这为智能体系统的持续扩展与自我改进提供了可行方案。

### 3. 对应检索需求
agents capable of self-improvement and autonomous skill acquisition。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=bwqwuJM68F](https://openreview.net/forum?id=bwqwuJM68F)
