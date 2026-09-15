---
title: "SEAgent: Self-Evolving Computer Use Agent with Autonomous Learning from Experience"
title_zh: SEAgent：具备自主经验学习的自进化电脑使用智能体
authors: "Zeyi Sun, Ziyu Liu, Yuhang Zang, Yuhang Cao, Xiaoyi Dong, Tong Wu, Dahua Lin, Jiaqi Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/82abdbced9d1bf9b03f3b3c2378f1567bec05198.pdf"
tags: ["query:self-evolve"]
score: 10.0
evidence: 自进化框架使智能体通过经验学习自主进化并掌握新软件
tldr: 针对大型视觉语言模型作为电脑使用智能体时依赖人工标注、难以适应陌生软件的问题，本文提出SEAgent自进化框架。该方法让智能体在与未知软件交互中通过试错进行经验学习，并逐步完成由简到繁自动生成的任务。实验表明智能体能在缺乏人工标注的场景下自主掌握新软件环境。该工作展示了智能体通过自主经验积累实现能力持续进化的可行路径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有电脑使用智能体依赖人工标注数据，难以应对缺乏标注的新颖专用软件。
method: 提出SEAgent自进化框架，让智能体探索新软件、迭代试错并渐进完成自动生成任务。
result: 智能体可在无人工标注条件下自主掌握陌生软件环境并逐步提升任务难度。
conclusion: 该工作验证了通过自主经验学习实现智能体能力持续自进化的可行性。
---

## Abstract
Repurposing large vision-language models (LVLMs) as computer use agents (CUAs) has led to substantial breakthroughs, primarily driven by human-labeled data. However, these models often struggle with novel and specialized software, particularly in scenarios lacking human annotations. To address this challenge, we propose SEAgent, an agentic self-evolving framework enabling CUAs to autonomously evolve through interactions with unfamiliar software. Specifically, SEAgent empowers computer-use agents to autonomously master novel software environments via experiential learning, where agents explore new software, learn through iterative trial-and-error, and progressively tackle auto-generated tasks organized from simple to complex. To achieve this goal, we design a World State Model for step-wise trajectory assessment, along with a Curriculum Generator that generates increasingly diverse and challenging tasks. The agent's policy is updated through experiential learning, comprised of adversarial imitation of failure actions and Group Relative Policy Optimization (GRPO) on successful ones. Furthermore, we introduce a specialist-to-generalist training strategy that integrates individual experiential insights from specialist agents, facilitating the development of a stronger generalist CUA capable of continuous autonomous evolution. This unified agent ultimately achieves performance surpassing ensembles of individual specialist agents on their specialized software. We validate the effectiveness of SEAgent across five professional software of OSWorld, ScienceBoard and AndroidWorld. Our approach achieves a significant improvement over a competitive open-source CUA, UI-TARS. All the code and models will be made publicly available to foster further research.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自进化框架使智能体通过经验学习自主进化并掌握新软件。

### 2. 核心内容
针对大型视觉语言模型作为电脑使用智能体时依赖人工标注、难以适应陌生软件的问题，本文提出SEAgent自进化框架。该方法让智能体在与未知软件交互中通过试错进行经验学习，并逐步完成由简到繁自动生成的任务。实验表明智能体能在缺乏人工标注的场景下自主掌握新软件环境。该工作展示了智能体通过自主经验积累实现能力持续进化的可行路径。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=AvBgmOGsdQ](https://openreview.net/forum?id=AvBgmOGsdQ)
