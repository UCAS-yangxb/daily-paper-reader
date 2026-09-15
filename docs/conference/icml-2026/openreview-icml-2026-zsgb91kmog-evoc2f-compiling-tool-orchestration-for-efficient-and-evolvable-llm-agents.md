---
title: "EvoC2F: Compiling Tool Orchestration for Efficient and Evolvable LLM Agents"
title_zh: EvoC2F：为高效可进化LLM智能体编译工具编排
authors: "Lei Wei, Qi Liu, Ruiyang Huang, Xiao Peng, Sicong Xie, Lanbo Lin, Chenhao Jiang, Yuanwu Xu, Tianyuan Yang, Jiayao Liu, Li Cai, Zhaolu Kang, Bin Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/380f8559a85365b000eaead09c96b5e737e24667.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 可进化的LLM智能体与可验证持续学习
tldr: 工具增强的语言模型智能体难以兼顾规划灵活性与生产部署可靠性，且从经验学习中常出现技能库污染，未经验证的抽象会随时间降低性能。本文提出EvoC2F框架，将工具编排重定义为程序编译，把规划约束到带语义标注的中间表示，并支持经验证的持续学习。该设计在保持效率的同时实现可进化的LLM智能体，缓解技能库污染，提升长期可靠性。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 工具增强LLM智能体难以兼顾规划灵活性与可靠性，且技能库易被污染。
method: 将工具编排编译为带语义标注的中间表示，并支持经验证的持续学习。
result: 在保持效率的同时实现可进化智能体，缓解技能库污染。
conclusion: 为LLM智能体的持续进化与可靠部署提供编译式框架。
---

## Abstract
Tool-augmented language model agents have shown great potential in solving complex real-world tasks, but a key challenge remains balancing planning flexibility with the reliability required for production deployment. Existing approaches either execute tools sequentially without parallelism or generate unconstrained code, hindering optimization and verification. Additionally, agents that learn from experience often suffer from skill library pollution, where unverified abstractions degrade performance over time. We propose EvoC2F, a framework that redefines tool orchestration through program compilation and verified continuous learning. By constraining plan generation to a well-defined intermediate representation with explicit semantic annotations, EvoC2F enables provably correct optimizations, parallelism, and fault tolerance, while ensuring soundness guarantees. Our verification-gated code-to-function evolution process ensures that learned skills undergo rigorous testing before library admission. Experiments across diverse benchmarks demonstrate that EvoC2F outperforms existing methods, reducing latency and establishing a robust foundation for building reliable, evolving autonomous agents.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
可进化的LLM智能体与可验证持续学习。

### 2. 核心内容
工具增强的语言模型智能体难以兼顾规划灵活性与生产部署可靠性，且从经验学习中常出现技能库污染，未经验证的抽象会随时间降低性能。本文提出EvoC2F框架，将工具编排重定义为程序编译，把规划约束到带语义标注的中间表示，并支持经验证的持续学习。该设计在保持效率的同时实现可进化的LLM智能体，缓解技能库污染，提升长期可靠性。

### 3. 对应检索需求
large language model based agents with self-evolution capabilities。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=ZSGB91kMOG](https://openreview.net/forum?id=ZSGB91kMOG)
