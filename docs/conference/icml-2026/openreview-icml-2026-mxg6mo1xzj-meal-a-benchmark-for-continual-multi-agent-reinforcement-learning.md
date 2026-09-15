---
title: "MEAL: A Benchmark for Continual Multi-Agent Reinforcement Learning"
title_zh: MEAL：持续多智能体强化学习基准
authors: "Tristan Tomilin, Luka van den Boogaard, Samuel Garcin, Constantin Ruhdorfer, Bram Grooten, Fabrice Kusters, Yali Du, Andreas Bulling, Mykola Pechenizkiy, Meng Fang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/f7ee900e02da7357f11c62a903340308441d51d4.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 首个持续多智能体强化学习基准，支撑终身学习
tldr: 终身学习虽受关注，但持续强化学习研究通常只涉及少量任务，且合作多智能体场景下的持续学习仍鲜有探索。作者提出MEAL，首个持续多智能体强化学习基准，借助JAX与GPU加速可在单卡上数小时内训练100个任务序列。实验发现长任务序列会暴露短序列中不出现的失败模式，为多智能体持续适应研究提供了可扩展评测平台。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 持续强化学习研究任务数少，合作多智能体场景下的持续学习鲜有探索。
method: 提出首个持续多智能体强化学习基准，利用JAX与GPU加速支持长任务序列。
result: 可在单卡数小时内训练100任务，暴露长序列特有的失败模式。
conclusion: 为多智能体终身学习与持续适应研究提供可扩展评测平台。
---

## Abstract
Benchmarks play a central role in reinforcement learning (RL) research, yet their computational constraints often shape what is studied. Despite the motivation of lifelong learning, most continual RL papers consider only 3–10 sequential tasks, as CPU-bound environments make longer sequences impractical. Meanwhile, continual learning in cooperative multi-agent settings remains largely unexplored. To address these gaps, we introduce **MEAL** (**M**ulti-agent **E**nvironments for **A**daptive **L**earning), the first benchmark for continual multi-agent RL. By leveraging JAX and GPU acceleration, MEAL enables training on sequences of 100 tasks on a single GPU in a few hours. We find that long task sequences reveal failure modes that do not appear at smaller scales.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
首个持续多智能体强化学习基准，支撑终身学习。

### 2. 核心内容
终身学习虽受关注，但持续强化学习研究通常只涉及少量任务，且合作多智能体场景下的持续学习仍鲜有探索。作者提出MEAL，首个持续多智能体强化学习基准，借助JAX与GPU加速可在单卡上数小时内训练100个任务序列。实验发现长任务序列会暴露短序列中不出现的失败模式，为多智能体持续适应研究提供了可扩展评测平台。

### 3. 对应检索需求
lifelong learning and continual adaptation in artificial agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=Mxg6mo1Xzj](https://openreview.net/forum?id=Mxg6mo1Xzj)
