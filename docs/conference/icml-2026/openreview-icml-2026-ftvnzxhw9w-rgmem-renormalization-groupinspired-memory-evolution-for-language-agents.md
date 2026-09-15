---
title: "RGMem: Renormalization Group–inspired Memory Evolution for Language Agents"
title_zh: RGMem：受重整化群启发的语言智能体记忆演化
authors: "Ao Tian, Yunfeng Lu, Xinxin Fan, Changhao Wang, Lanzhi Zhou, Yeyao Zhang, Yanfang Liu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a9944c66058e0655a6bd75242b0d62071a06444d.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 面向语言智能体的自进化记忆框架
tldr: 针对有限上下文窗口与静态参数记忆难以建模跨会话长期用户状态的问题，本文提出自进化记忆框架RGMem。受重整化群多尺度组织与涌现思想启发，该方法将长期对话记忆建模为多尺度演化过程，把片段化交互逐级转化为稳定偏好与深层用户特征。实验表明其能在演化且可能冲突的对话中提炼稳定用户画像，为语言智能体的长期个性化记忆提供了自进化机制。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 有限上下文与静态记忆难以从演化对话中提炼稳定的长期用户状态。
method: 提出RGMem，以重整化群多尺度视角把长期对话记忆建模为演化过程。
result: 能从演化且可能冲突的对话中提炼稳定偏好与深层用户特征。
conclusion: 为语言智能体的长期个性化记忆提供了自进化式多尺度建模机制。
---

## Abstract
Personalized and continuous interactions are critical for LLM-based conversational agents, yet finite context windows and static parametric memory hinder the modeling of long-term, cross-session user states. Existing approaches, including retrieval-augmented generation and explicit memory systems, primarily operate at the fact level, making it difficult to distill stable preferences and deep user traits from evolving and potentially conflicting dialogues.To address this challenge, we propose RGMem, a self-evolving memory framework inspired by the renormalization group (RG) perspective on multi-scale organization and emergence. RGMem models long-term conversational memory as a multi-scale evolutionary process: episodic interactions are transformed into semantic facts and user insights, which are then progressively integrated through hierarchical coarse-graining, thresholded updates, and rescaling into a dynamically evolving user profile.By explicitly separating fast-changing evidence from slow-varying traits and enabling non-linear, phase-transition-like dynamics, RGMem enables robust personalization beyond flat retrieval or static summarization. Extensive experiments on the LOCOMO and PersonaMem benchmarks demonstrate that RGMem consistently outperforms SOTA memory systems, achieving stronger cross-session continuity and improved adaptation to evolving user preferences.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向语言智能体的自进化记忆框架。

### 2. 核心内容
针对有限上下文窗口与静态参数记忆难以建模跨会话长期用户状态的问题，本文提出自进化记忆框架RGMem。受重整化群多尺度组织与涌现思想启发，该方法将长期对话记忆建模为多尺度演化过程，把片段化交互逐级转化为稳定偏好与深层用户特征。实验表明其能在演化且可能冲突的对话中提炼稳定用户画像，为语言智能体的长期个性化记忆提供了自进化机制。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=FtvNZxhW9W](https://openreview.net/forum?id=FtvNZxhW9W)
