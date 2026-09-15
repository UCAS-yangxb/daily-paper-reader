---
title: Decision Transformers As Zero-Shot Learners via Text-Behavior Alignment
title_zh: 决策Transformer作为零样本学习者：通过文本-行为对齐
authors: "Xin Zhang, Jonathan Martinez, Yanhua Li, Yingxue Zhang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/4cb3caff415a366453ebd17987cf80d2724e0590.pdf"
tags: ["query:self-evolve"]
score: 5.0
evidence: 离线元强化学习实现基于语言的零样本任务适应
tldr: 离线元强化学习通常依赖目标任务的演示数据来实现适应，但现实中往往只有任务目标而无演示。作者探索用自然语言任务描述实现零样本任务适应，提出将决策Transformer与文本-行为对齐相结合的方法，无需目标任务的任何数据。实验表明智能体仅凭语言指令即可适应新任务，为元学习驱动的智能体行为迁移提供了新途径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 离线元强化学习依赖目标演示数据，现实中往往只有语言任务目标而无可演示。
method: 提出文本-行为对齐方法，用自然语言描述驱动决策Transformer实现零样本适应。
result: 智能体无需目标数据即可凭语言指令适应新任务。
conclusion: 展示了元学习结合语言指令可扩展智能体的任务适应能力。
---

## Abstract
Offline meta-reinforcement learning (meta-RL) aims to train agents that can generalize to unseen tasks using pre-collected data from related tasks. Recent approaches leverage the scalability of transformer architectures to model behavior sequences and support task adaptation using target task demonstrations. However, such data is often unavailable in real-world settings, where the task objective may be known but cannot be easily demonstrated. In contrast, humans routinely interpret and perform new tasks based solely on natural language instructions. In this work, we explore the potential of using natural language task descriptions to enable zero-shot task adaptation in offline meta-RL without requiring any data from the target task. We propose the Text-Guided Decision Transformer (TG-DT), a framework that enables zero-shot generalization by grounding policy learning in natural language. TG-DT learns a shared embedding space between task descriptions and behavioral trajectories via a dual contrastive and matching-based objective, ensuring robust alignment. A transformer-based policy is then conditioned on these aligned representations to generate task-appropriate actions. At test time, TG-DT synthesizes policies for unseen tasks using only their text descriptions and can optionally leverage a description-guided data sharing strategy to enhance adaptation. Experiments on standard offline meta-RL benchmarks, including MuJoCo and Meta-World, demonstrate that TG-DT achieves strong generalization to unseen tasks.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
离线元强化学习实现基于语言的零样本任务适应。

### 2. 核心内容
离线元强化学习通常依赖目标任务的演示数据来实现适应，但现实中往往只有任务目标而无演示。作者探索用自然语言任务描述实现零样本任务适应，提出将决策Transformer与文本-行为对齐相结合的方法，无需目标任务的任何数据。实验表明智能体仅凭语言指令即可适应新任务，为元学习驱动的智能体行为迁移提供了新途径。

### 3. 对应检索需求
self improvement and meta learning techniques for evolving agent behaviors。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=jqLPUccarO](https://openreview.net/forum?id=jqLPUccarO)
