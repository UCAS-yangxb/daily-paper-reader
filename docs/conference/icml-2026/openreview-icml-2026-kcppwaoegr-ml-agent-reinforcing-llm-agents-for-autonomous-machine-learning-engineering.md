---
title: "ML-Agent: Reinforcing LLM Agents for Autonomous Machine Learning Engineering"
title_zh: ML-Agent：强化LLM智能体实现自主机器学习工程
authors: "Zexi Liu, Jingyi Chai, Xinyu Zhu, Shuo Tang, Rui Ye, Weiyu Ma, Bo Zhang, LEI BAI, Siheng Chen"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/aad5c8df9dbe56e96769be57e2b17c6f7444eca5.pdf"
tags: ["query:self-evolve"]
score: 6.0
evidence: LLM智能体通过在线强化学习交互实验自我提升
tldr: 现有基于提示的LLM智能体范式存在局限：小模型无法从执行轨迹中学习泛化，大模型开销高。作者首次探索基于学习的智能体式机器学习范式，让LLM智能体通过在线强化学习在ML任务上交互实验并自我提升，框架包含探索增强微调等关键组件。实验显示该智能体能自主习得并改进ML工程能力，为可自我进化的智能体提供了训练范式。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 提示式LLM智能体难以从轨迹中学习泛化且大模型开销高，限制可扩展性。
method: 提出基于在线强化学习的智能体式ML训练框架，含探索增强微调等组件。
result: 智能体通过交互实验自主提升ML任务表现，降低对提示式大模型的依赖。
conclusion: 验证了学习式智能体范式可让LLM智能体自主进化能力。
---

## Abstract
The emergence of large language model (LLM)-based agents has significantly advanced the development of autonomous machine learning (ML) engineering. However, the dominant prompt-based paradigm exhibits limitations: smaller models lack the capacity to learn from execution trajectories for generalization, while large proprietary models incur high computational overhead, restricting accessibility and scalability. Focusing on this, for the first time, we explore the paradigm of learning-based agentic ML, where an LLM agent learns through interactive experimentation on ML tasks using online reinforcement learning (RL). To realize this, we propose a novel agentic ML training framework with three key components: (1) exploration-enriched fine-tuning, which enables LLM agents to generate diverse actions for enhanced RL exploration; (2) step-wise RL, which enables training on a single action step, accelerating experience collection and improving training efficiency; (3) an agentic ML-specific reward module, which unifies varied ML feedback signals into consistent rewards for RL optimization. Leveraging this framework, we train ML-Agent, driven by a 7B-sized Qwen-2.5 LLM for autonomous ML. Despite training on only 9 ML tasks, our 7B-sized ML-Agent achieves comparable performance to agents using much larger proprietary LLMs (e.g., GPT-5) but at significantly lower computational cost, demonstrating strong performance and cross-task generalization.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
LLM智能体通过在线强化学习交互实验自我提升。

### 2. 核心内容
现有基于提示的LLM智能体范式存在局限：小模型无法从执行轨迹中学习泛化，大模型开销高。作者首次探索基于学习的智能体式机器学习范式，让LLM智能体通过在线强化学习在ML任务上交互实验并自我提升，框架包含探索增强微调等关键组件。实验显示该智能体能自主习得并改进ML工程能力，为可自我进化的智能体提供了训练范式。

### 3. 对应检索需求
agents capable of self-improvement and autonomous skill acquisition。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=kcPPWaoegr](https://openreview.net/forum?id=kcPPWaoegr)
