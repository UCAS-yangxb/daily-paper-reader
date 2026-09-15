---
title: "AdaMEM: Test-Time Adaptive Memory for Language Agents"
title_zh: AdaMEM：面向语言智能体的测试时自适应记忆
authors: "Yunxiang Zhang, Yiheng Li, Ali Payani, Lu Wang"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/60e7619ab7b16364061f0571b8a63f278434cf41.pdf"
tags: ["query:self-evolve"]
score: 8.0
evidence: 测试时自适应记忆持续适应
tldr: 语言智能体难以利用过往经验适应动态测试条件，多数记忆机制仅在情节开始检索，导致长时程任务中指导逐渐失配。本文提出AdaMEM，通过混合记忆架构在不更新参数的情况下实现测试时自适应：维护长期轨迹记忆并即时生成动态短期策略记忆。该机制提升智能体在长时程任务中的决策表现。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 语言智能体难以利用过往经验适应动态测试条件，检索多限于情节开始导致指导失配。
method: 提出AdaMEM，通过混合记忆架构在不更新参数下生成动态短期策略记忆。
result: 结合长期轨迹记忆与动态策略记忆，引导长时程决策。
conclusion: 实现智能体测试时自适应，提升长时程任务表现。
---

## Abstract
A central challenge for language agents is utilizing past experience to adapt to dynamic test-time conditions. While recent work demonstrates the promise of agentic memory mechanisms, most systems restrict retrieval to episode initiation. Consequently, agents are forced to rely on static guidance that becomes increasingly misaligned as long-horizon tasks unfold.
To address this rigidity, we propose the Adaptive Memory Agent (AdaMEM), a novel framework for agent test-time adaptation. Without updating model parameters online, AdaMEM adapts agent behavior via a hybrid memory architecture: it maintains a long-term trajectory memory of raw experiences collected offline while generating dynamic short-term strategy memory on-the-fly to guide decision-making.
This mechanism enables the trade-off between token efficiency and adaptability across varying inference-time compute levels. Empirically, AdaMEM significantly outperforms static memory baselines, achieving relative gains of up to 13% on ALFWorld and 11% on WebShop, with consistent leading performance extending to agentic search on HotpotQA.
To further enhance this adaptation, we develop Step-MFT, a Step-wise Memory Fine-Tuning technique that trains the policy to synthesize high-quality strategies from retrieved experiences, yielding additional performance gains. 
Our work establishes a new scaling dimension for agentic memory, supporting continuous reasoning and self-evolution post-deployment in real-world environments. Our code is available at https://github.com/yunx-z/AdaMEM.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
测试时自适应记忆持续适应。

### 2. 核心内容
语言智能体难以利用过往经验适应动态测试条件，多数记忆机制仅在情节开始检索，导致长时程任务中指导逐渐失配。本文提出AdaMEM，通过混合记忆架构在不更新参数的情况下实现测试时自适应：维护长期轨迹记忆并即时生成动态短期策略记忆。该机制提升智能体在长时程任务中的决策表现。

### 3. 对应检索需求
lifelong learning and continual adaptation in artificial agents。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=RzlmkviaNy](https://openreview.net/forum?id=RzlmkviaNy)
