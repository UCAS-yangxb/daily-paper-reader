---
title: Toward Training Superintelligent Software Agents through Self-Play SWE-RL
title_zh: 通过自博弈软件工程强化学习训练超级智能软件智能体
authors: "Yuxiang Wei, Zhiqing Sun, Emily McMilin, Jonas Gehring, David W. Zhang, Gabriel Synnaeve, Daniel Fried, LINGMING ZHANG, Sida Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/9dabda3b0f1dc69bcb238b2447427a6560b97075.pdf"
tags: ["query:self-evolve"]
score: 7.0
evidence: 自博弈强化学习智能体自主提升
tldr: 现有基于大模型与强化学习的软件智能体依赖人工标注数据与环境，成为通往超级智能的障碍。本文提出Self-play SWE-RL，仅需沙箱代码仓库，让单个智能体在自博弈中注入并修复日益复杂的缺陷，并由测试套件改进正式定义缺陷。实验表明无需人工标注即可在真实代码库中持续提升能力，为最小数据假设下训练自进化软件智能体开辟了路径。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 现有软件智能体依赖人工标注的训练数据与环境，构成通往超级智能的根本障碍。
method: 提出Self-play SWE-RL，仅需沙箱代码仓库，让单个LLM智能体在自博弈中注入并修复日益复杂的缺陷。
result: 智能体在真实代码库中通过自博弈生成训练信号，无需人工标注即可持续提升能力。
conclusion: 为最小数据假设下训练自进化软件智能体提供了可行路径。
---

## Abstract
While current software agents powered by large language models (LLMs) and reinforcement learning (RL) can boost programmer productivity, their reliance on human-curated training data and environments creates a fundamental barrier to superintelligence. In this paper, we present Self-play SWE-RL (SSR), a first step toward training superintelligent software agents under minimal data assumptions. SSR requires only access to sandboxed repositories with source code and dependencies, no need for human-labeled issues or test commands. Grounded in real-world codebases, a single LLM agent is trained via RL in a self-play setting to inject and repair increasingly complex bugs. The bugs are formally specified by test suite improvements proposed by the agent rather than natural language issue descriptions. On the SWE-bench Verified and SWE-Bench Pro benchmarks, SSR achieves clear self-improvement (+10.4 and +7.8 points) and consistently outperforms the human-data baseline throughout training, generalizing to natural language bug descriptions not seen in training. Overall, our results point toward a paradigm where agents autonomously gather extensive learning experiences from real software repositories, ultimately enabling superintelligent systems that exceed human capabilities in understanding, modifying, and creating software from scratch.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自博弈强化学习智能体自主提升。

### 2. 核心内容
现有基于大模型与强化学习的软件智能体依赖人工标注数据与环境，成为通往超级智能的障碍。本文提出Self-play SWE-RL，仅需沙箱代码仓库，让单个智能体在自博弈中注入并修复日益复杂的缺陷，并由测试套件改进正式定义缺陷。实验表明无需人工标注即可在真实代码库中持续提升能力，为最小数据假设下训练自进化软件智能体开辟了路径。

### 3. 对应检索需求
agents capable of self-improvement and autonomous skill acquisition。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=0ophJB76sC](https://openreview.net/forum?id=0ophJB76sC)
