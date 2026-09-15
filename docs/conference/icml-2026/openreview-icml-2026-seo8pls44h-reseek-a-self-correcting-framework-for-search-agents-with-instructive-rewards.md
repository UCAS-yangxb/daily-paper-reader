---
title: "ReSeek: A Self-Correcting Framework for Search Agents with Instructive Rewards"
title_zh: ReSeek：面向搜索智能体的自校正框架与指导性奖励
authors: "Shiyu Li, Yifan Wang, Peiming Li, Zheng Wei, Yang Tang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/594d22dfbdb114617022d4020ce5d747193040a8.pdf"
tags: ["query:self-evolve"]
score: 4.0
evidence: 智能体自适应纠错恢复
tldr: 基于大语言模型的搜索智能体在多步推理中易因稀疏奖励固守错误路径而难以恢复。作者提出ReSeek自校正框架，通过引入JUDGE动作让智能体判断信息并重新规划搜索策略，并设计稠密的指导性奖励引导该过程。该机制使智能体能在单次任务中从错误搜索路径中恢复。研究提升了搜索智能体多步推理的鲁棒性与可靠性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 基于强化学习的搜索智能体常因稀疏或规则化奖励而陷入错误推理路径且无法自行恢复。
method: 提出ReSeek自校正框架，通过JUDGE动作判断信息并重新规划搜索策略，并设计稠密的指导性奖励引导该过程。
result: 使搜索智能体能在单次任务内从错误的搜索路径中恢复，提升多步推理稳定性。
conclusion: 为提升搜索智能体多步推理的鲁棒性提供了自校正机制。
---

## Abstract
Search agents powered by Large Language Models have demonstrated significant potential in tackling knowledge-intensive tasks. Reinforcement learning has emerged as a powerful paradigm for training these agents to perform complex, multi-step reasoning. However, prior RL-based methods often rely on sparse or rule-based rewards, which can lead agents to commit to suboptimal or erroneous reasoning paths without the ability to recover. To address these limitations, we propose **ReSeek**, a self-correcting framework enabling search agents to recover from erroneous search paths during an episode. By invoking a special **JUDGE** action, the agent can judge the information and re-plan its search strategy. To guide this process, we design a dense, instructive process reward function, which decomposes into a correctness reward for retrieving factual information and a utility reward for finding information genuinely useful for the query. Additionally, to mitigate the risk of data contamination in existing datasets, we introduce **FictionalHot**, a contamination-free benchmark requiring complex reasoning. Experiments show ReSeek significantly outperforms SOTA baselines in task success and path faithfulness.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
智能体自适应纠错恢复。

### 2. 核心内容
基于大语言模型的搜索智能体在多步推理中易因稀疏奖励固守错误路径而难以恢复。作者提出ReSeek自校正框架，通过引入JUDGE动作让智能体判断信息并重新规划搜索策略，并设计稠密的指导性奖励引导该过程。该机制使智能体能在单次任务中从错误搜索路径中恢复。研究提升了搜索智能体多步推理的鲁棒性与可靠性。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=SeO8pLS44H](https://openreview.net/forum?id=SeO8pLS44H)
