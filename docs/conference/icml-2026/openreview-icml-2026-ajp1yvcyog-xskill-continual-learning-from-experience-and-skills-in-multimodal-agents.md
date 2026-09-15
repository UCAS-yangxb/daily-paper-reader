---
title: "XSkill: Continual Learning from Experience and Skills in Multimodal Agents"
title_zh: XSkill：多模态智能体从经验与技能中持续学习
authors: "Guanyu Jiang, Zhaochen Su, Xiaoye Qu, Yi R. Fung"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/d2d53316f305c31624bb729a7b76925398cbb925.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 无需参数更新的经验与技能持续学习
tldr: 多模态智能体在开放式场景中常面临工具使用低效和编排不灵活的问题，亟需在不更新参数的情况下从历史轨迹中持续改进。作者提出XSkill双流框架，区分经验（动作级指导）与技能（任务级指导）两种可复用知识，并基于视觉观察进行知识提取与检索。实验表明该方法能提升多模态智能体的工具使用与规划能力。该工作为智能体的持续学习与自我进化提供了新范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多模态智能体在开放场景中工具使用低效、编排不灵活，需在不更新参数的前提下从历史轨迹持续改进。
method: 提出XSkill双流框架，区分经验与技能两种可复用知识，并基于视觉观察进行知识提取与检索。
result: 提升了多模态智能体在开放任务中的工具使用与规划能力。
conclusion: 为无需参数更新的智能体持续学习提供了新范式。
---

## Abstract
Multimodal agents can now tackle complex reasoning tasks with diverse tools, yet they still suffer from inefficient tool use and inflexible orchestration in open-ended settings. A central challenge is enabling such agents to continually improve without parameter updates by learning from past trajectories. We identify two complementary forms of reusable knowledge essential for this goal: experiences, providing concise action-level guidance for tool selection and decision making, and skills, providing structured task-level guidance for planning and tool use. To this end, we propose XSkill, a dual-stream framework for continual learning from experience and skills in multimodal agents. XSkill grounds both knowledge extraction and retrieval in visual observations. During accumulation, XSkill distills and consolidates experiences and skills from multi-path rollouts via visually grounded summarization and cross-rollout critique. During inference, it retrieves and adapts this knowledge to the current visual context and feeds usage history back into accumulation to form a continual learning loop. Evaluated on five benchmarks across diverse domains with four backbone models, XSkill consistently and substantially outperforms both tool-only and learning-based baselines. Further analysis reveals that the two knowledge streams play complementary roles in influencing the reasoning behaviors of agents and show superior zero-shot generalization. Code is available at https://github.com/XSkill-Agent/XSkill.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
无需参数更新的经验与技能持续学习。

### 2. 核心内容
多模态智能体在开放式场景中常面临工具使用低效和编排不灵活的问题，亟需在不更新参数的情况下从历史轨迹中持续改进。作者提出XSkill双流框架，区分经验（动作级指导）与技能（任务级指导）两种可复用知识，并基于视觉观察进行知识提取与检索。实验表明该方法能提升多模态智能体的工具使用与规划能力。该工作为智能体的持续学习与自我进化提供了新范式。

### 3. 对应检索需求
methods for lifelong learning and continual adaptation in autonomous intelligent agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=AjP1yvCyoG](https://openreview.net/forum?id=AjP1yvCyoG)
