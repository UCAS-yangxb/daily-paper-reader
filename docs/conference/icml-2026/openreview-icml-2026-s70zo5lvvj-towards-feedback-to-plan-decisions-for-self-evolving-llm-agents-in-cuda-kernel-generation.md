---
title: Towards Feedback-to-Plan Decisions for Self-Evolving LLM Agents in CUDA Kernel Generation
title_zh: 面向CUDA核生成中自进化大模型智能体的反馈到规划决策
authors: "Yee Hin Chong, Jiaming Wu, Youhui Zhang, Peng Qu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/86238cbeafc0b1dec4be15150a6131916dc449af.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 面向CUDA核生成的自进化大模型智能体分析
tldr: 针对自进化LLM智能体在CUDA核生成中如何归因并融合异构反馈信号仍不透明的问题，本文提出CUDAnalyst统一分析层。它通过轨迹冻结与选择性反馈注入，实现生成级别的受控归因，从而稳定评估反馈各成分对规划决策的贡献。该工作揭示了迭代规划中早期扰动放大与漂移干扰的问题，为自进化智能体的反馈驱动规划机制提供了可解释、可分析的方法支撑。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自进化LLM智能体如何归因并组合异构反馈信号进行规划仍不透明。
method: 提出CUDAnalyst，用轨迹冻结与选择性反馈注入实现生成级受控归因分析。
result: 实现稳定的生成级评估，厘清各反馈成分对规划决策的贡献。
conclusion: 为自进化智能体的反馈驱动规划机制提供了可解释的分析层。
---

## Abstract
Large language models (LLMs) have shown strong empirical gains as self-evolving agents for CUDA kernel generation, driven by feedback-conditioned planning across generations. However, how planning decisions attribute and combine heterogeneous feedback signals remains opaque. Standard end-to-end ablations fail to resolve this question, as iterative planning amplifies early perturbations and conflates feedback effects with trajectory-dependent drift.

We introduce \texttt{CUDAnalyst}, a unified analysis layer for controlled, generation-level attribution of planning decisions to feedback components via trajectory freezing and selective feedback injection. \texttt{CUDAnalyst} enables stable generation-level evaluation and principled coalitional-style attribution of feedback effects and interactions. Our results show that explicit planning is beneficial only when feedback is aligned, that effective planning emerges from structured multi-feedback interactions, and that high-level plans from stronger reasoning models can partially transfer to weaker ones. These trends hold across reference backbones, representative workloads, and reference induction regimes, indicating that the identified feedback-to-plan structure is robust within the controlled axes studied.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
面向CUDA核生成的自进化大模型智能体分析。

### 2. 核心内容
针对自进化LLM智能体在CUDA核生成中如何归因并融合异构反馈信号仍不透明的问题，本文提出CUDAnalyst统一分析层。它通过轨迹冻结与选择性反馈注入，实现生成级别的受控归因，从而稳定评估反馈各成分对规划决策的贡献。该工作揭示了迭代规划中早期扰动放大与漂移干扰的问题，为自进化智能体的反馈驱动规划机制提供了可解释、可分析的方法支撑。

### 3. 对应检索需求
large language model based agents with self-evolution capabilities。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=s70zO5Lvvj](https://openreview.net/forum?id=s70zO5Lvvj)
