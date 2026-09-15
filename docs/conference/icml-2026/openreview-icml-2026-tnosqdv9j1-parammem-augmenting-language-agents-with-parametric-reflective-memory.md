---
title: "ParamMem: Augmenting Language Agents with Parametric Reflective Memory"
title_zh: ParamMem：为语言智能体增强参数化反思记忆
authors: "Tianjun Yao, Yongqiang Chen, Yujia Zheng, Pan Li, Zhiqiang Shen, Kun Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a8f8d44c9fbeda54d0be37feb00e39fa531c146f.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 自反思智能体迭代精炼解决方案
tldr: 自反思能让语言智能体迭代改进解决方案，但常产生重复输出，限制推理性能。本文发现反思多样性与任务成功高度正相关，据此提出参数化记忆模块ParamMem，将跨样本的反思模式编码进模型参数，通过温度采样生成多样反思。基于该模块的ParamAgent在推理任务上取得提升，为语言智能体通过多样化自我反思实现自我改进提供了新机制。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自反思智能体常产生重复输出，限制推理性能与自我改进效果。
method: 提出ParamMem参数化记忆模块编码跨样本反思模式，并构建ParamAgent框架。
result: 通过温度采样生成多样反思，提升推理表现。
conclusion: 为语言智能体通过多样化自我反思实现自我改进提供新机制。
---

## Abstract
Self-reflection enables language agents to iteratively refine solutions, yet often produces repetitive outputs that limit reasoning performance. Recent studies have attempted to address this limitation through various approaches, among which increasing reflective diversity has shown promise. Our empirical analysis reveals a strong positive correlation between reflective diversity and task success, further motivating the need for diverse reflection signals. We introduce `ParamMem`, a parametric memory module that encodes cross-sample reflection patterns into model parameters, enabling diverse reflection generation through temperature-controlled sampling. Building on this module, we propose ParamAgent, a reflection-based agent framework that integrates parametric memory with episodic and cross-sample memory. Extensive experiments on code generation, mathematical reasoning, and multi-hop question answering demonstrate consistent improvements over state-of-the-art baselines. Further analysis reveals that `ParamMem` is sample-efficient, enables weak-to-strong transfer across model scales, and supports self-improvement without reliance on stronger external model, highlighting the potential of `ParamMem` as an effective component for enhancing language agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自反思智能体迭代精炼解决方案。

### 2. 核心内容
自反思能让语言智能体迭代改进解决方案，但常产生重复输出，限制推理性能。本文发现反思多样性与任务成功高度正相关，据此提出参数化记忆模块ParamMem，将跨样本的反思模式编码进模型参数，通过温度采样生成多样反思。基于该模块的ParamAgent在推理任务上取得提升，为语言智能体通过多样化自我反思实现自我改进提供了新机制。

### 3. 对应检索需求
self improvement and meta learning techniques for evolving agent behaviors。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=tNosQdV9J1](https://openreview.net/forum?id=tNosQdV9J1)
