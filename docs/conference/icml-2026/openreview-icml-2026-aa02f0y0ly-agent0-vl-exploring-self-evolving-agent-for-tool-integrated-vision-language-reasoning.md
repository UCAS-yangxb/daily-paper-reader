---
title: "Agent0-VL: Exploring Self-Evolving Agent for Tool-Integrated Vision-Language Reasoning"
title_zh: Agent0-VL：探索面向工具集成视觉语言推理的自进化智能体
authors: "Jiaqi Liu, Kaiwen Xiong, Peng Xia, Yiyang Zhou, Haonian Ji, Lu Feng, Siwei Han, Mingyu Ding, Huaxiu Yao"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/a96029e86d7d6be8d22752d121b03b2eee56cb07.pdf"
tags: ["query:self-evolve"]
score: 9.0
evidence: 自进化视觉语言智能体持续改进
tldr: 大型视觉语言模型的学习受限于人工标注监督，纯文本自评难以验证复杂视觉推理步骤且易产生评估幻觉。本文提出Agent0-VL，一个自进化的视觉语言智能体，将工具使用融入推理与自我奖励。它在工具集成推理下实现持续改进，为多模态智能体自进化提供新方案。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LVLM学习受限于人工标注监督，纯文本自评难以验证复杂视觉推理。
method: 提出Agent0-VL自进化视觉语言智能体，将工具使用融入推理与自奖励。
result: 实现工具集成推理下的持续改进。
conclusion: 为多模态智能体自进化提供新方案。
---

## Abstract
Large Vision-Language Models (LVLMs) have achieved remarkable progress in multimodal reasoning tasks; however, their learning remains constrained by the limitations of human-annotated supervision. Recent self-rewarding approaches attempt to overcome this constraint by allowing models to act as their own critics or reward providers. Yet, purely text-based self-evaluation struggles to verify complex visual reasoning steps and often suffers from evaluation hallucinations. To address these challenges, inspired by recent advances in tool-integrated reasoning, we propose Agent0-VL, a self-evolving vision-language agent that achieves continual improvement with tool-integrated reasoning. Agent0-VL incorporates tool usage not only into reasoning but also into self-evaluation and self-repair, enabling the model to introspect, verify, and refine its reasoning through evidence-grounded analysis. It unifies two synergistic roles within a single LVLM: a Solver that performs multi-turn tool-integrated reasoning, and a Verifier that generates structured feedback and fine-grained self-rewards through tool-grounded critique. These roles interact through a Self-Evolving Reasoning Cycle, where tool-based verification and reinforcement learning jointly align the reasoning and evaluation distributions for stable self-improvement. Through this zero-external-reward evolution, Agent0-VL aligns its reasoning and verification behaviors without any human annotation or external reward models, achieving continual self-improvement. Experiments on chart reasoning, geometric problem solving, and visual scientific analysis show that Agent0-VL achieves an 12.5% improvement over the Qwen-VL base model.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自进化视觉语言智能体持续改进。

### 2. 核心内容
大型视觉语言模型的学习受限于人工标注监督，纯文本自评难以验证复杂视觉推理步骤且易产生评估幻觉。本文提出Agent0-VL，一个自进化的视觉语言智能体，将工具使用融入推理与自我奖励。它在工具集成推理下实现持续改进，为多模态智能体自进化提供新方案。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=aA02f0y0LY](https://openreview.net/forum?id=aA02f0y0LY)
