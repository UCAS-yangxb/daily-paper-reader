---
title: Safe and Scalable Web Agent Learning via Recreated Websites
title_zh: 通过重建网站实现安全且可扩展的网页智能体学习
authors: "Hyungjoo Chae, Jungsoo Park, Alan Ritter"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/c2afd1ace56b4878c7b02ffb5a7e124fa1ae83a3.pdf"
tags: ["query:self-evolve"]
score: 6.0
evidence: 重建网站通过环境扩展与自生成任务实现可扩展的自进化
tldr: 针对真实网站不安全、难以重置且缺乏可验证反馈而限制网页智能体训练的问题，本文提出VeriEnv框架。该方法将语言模型作为环境创建者，自动把真实网站克隆为可执行、可验证的合成环境，并通过Python SDK暴露受控内部访问，使智能体自生成任务并获得确定性奖励。实验表明该设计解耦了学习与不安全的真实交互，并通过环境扩展支持可扩展自进化。这为智能体的安全持续学习提供了新基础设施。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 真实网站不安全、难重置且缺乏可验证反馈，限制了网页智能体的训练。
method: 提出VeriEnv，用语言模型将真实网站克隆为可执行可验证的合成环境并支持任务自生成。
result: 该方法使智能体获得确定性奖励并解耦不安全交互，实现可扩展自进化。
conclusion: 重建可验证环境为智能体的安全持续学习提供了可扩展基础设施。
---

## Abstract
Training autonomous web agents is fundamentally limited by the environments they learn from: real-world websites are unsafe to explore, hard to reset, and rarely provide verifiable feedback.
We propose VeriEnv, a framework that treats language models as environment creators, automatically cloning real-world websites into fully executable, verifiable synthetic environments.
By exposing controlled internal access via a Python SDK, VeriEnv enables agents to self-generate tasks with deterministic, programmatically verifiable rewards, eliminating reliance on heuristic or LLM-based judges.
This design decouples agent learning from unsafe real-world interaction while enabling scalable self-evolution through environment expansion.
Through experiments on web agent benchmarks, we show that agents trained with VeriEnv generalize to unseen websites, achieve site-specific mastery through self-evolving training, and benefit from scaling the number of training environments.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
重建网站通过环境扩展与自生成任务实现可扩展的自进化。

### 2. 核心内容
针对真实网站不安全、难以重置且缺乏可验证反馈而限制网页智能体训练的问题，本文提出VeriEnv框架。该方法将语言模型作为环境创建者，自动把真实网站克隆为可执行、可验证的合成环境，并通过Python SDK暴露受控内部访问，使智能体自生成任务并获得确定性奖励。实验表明该设计解耦了学习与不安全的真实交互，并通过环境扩展支持可扩展自进化。这为智能体的安全持续学习提供了新基础设施。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=x1OLusJLNe](https://openreview.net/forum?id=x1OLusJLNe)
