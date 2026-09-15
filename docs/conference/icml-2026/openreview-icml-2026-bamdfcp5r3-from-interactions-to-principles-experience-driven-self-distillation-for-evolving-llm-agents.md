---
title: "From Interactions to Principles: Experience-Driven Self-Distillation for Evolving LLM Agents"
title_zh: 从交互到原则：面向进化型大模型智能体的经验驱动自蒸馏
authors: "Rong Wu, Xiaoman Wang, Jianbiao Mei, Pinlong Cai, Daocheng Fu, Cheng Yang, Licheng Wen, Xuemeng Yang, Yufan Shen, Yuxin Wang, Botian Shi"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/299092bd65df43b35f26fb412844384e58850601.pdf"
tags: ["query:self-evolve"]
score: 9.0
evidence: 经验驱动的自蒸馏框架使智能体利用自身历史进化
tldr: 针对多数LLM智能体在每轮任务后丢弃交互轨迹、无法积累可复用策略的问题，本文提出经验驱动的自蒸馏框架EvolveR。该框架维护一个由历史轨迹提炼出的策略原则经验库，在离线阶段让智能体把成功与失败轨迹自蒸馏为简洁原则，并在推理中加以应用。实验表明该机制能持续提升智能体表现，实现无需外部教师模型的自我进化，为构建可累积经验的自主智能体提供了有效范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 多数LLM智能体每轮任务后丢弃交互轨迹，无法积累可复用策略。
method: 提出EvolveR，将成功与失败轨迹自蒸馏为策略原则并维护经验库加以复用。
result: 智能体可借助自身交互历史持续改进策略，无需外部教师模型。
conclusion: 提供了一种基于自蒸馏经验积累的LLM智能体自我进化范式。
---

## Abstract
LLM agents have achieved strong performance in tool-augmented reasoning, but most remain largely stateless: after each episode, the agent discards interaction traces and does not accumulate reusable strategies. Prior work either stores raw trajectories for case-based reuse or relies on external teacher models to write reflections, which limits generalization or leaves the agent’s policy unchanged. We introduce EvolveR, an experience-driven framework that allows an agent to improve using its own interaction history. EvolveR maintains an experience base of distilled strategic principles derived from past trajectories. In an offline phase, the agent self-distills successful and failed trajectories into concise principles, applies semantic deduplication, and assigns each principle an empirical utility score for maintenance and pruning. In an online phase, the agent retrieves top-ranked principles to guide reasoning and tool usage, generating new trajectories. We then perform policy evolution with reinforcement learning on these experience-conditioned trajectories, reinforcing behaviors that effectively retrieve and apply useful principles. We demonstrate the effectiveness of EvolveR on complex multi-hop question-answering benchmarks, where it achieves superior performance over strong agentic baselines. Our work presents a comprehensive blueprint for agents that learn not only from external data but also from the consequences of their own actions, paving the way for more autonomous and continuously improving systems.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
经验驱动的自蒸馏框架使智能体利用自身历史进化。

### 2. 核心内容
针对多数LLM智能体在每轮任务后丢弃交互轨迹、无法积累可复用策略的问题，本文提出经验驱动的自蒸馏框架EvolveR。该框架维护一个由历史轨迹提炼出的策略原则经验库，在离线阶段让智能体把成功与失败轨迹自蒸馏为简洁原则，并在推理中加以应用。实验表明该机制能持续提升智能体表现，实现无需外部教师模型的自我进化，为构建可累积经验的自主智能体提供了有效范式。

### 3. 对应检索需求
self-evolving agents that autonomously improve their capabilities over time。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=BamDfCP5R3](https://openreview.net/forum?id=BamDfCP5R3)
