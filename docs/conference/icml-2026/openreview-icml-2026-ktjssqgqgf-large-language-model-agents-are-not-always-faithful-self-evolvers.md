---
title: Large Language Model Agents Are Not Always Faithful Self-Evolvers
title_zh: 大语言模型智能体并非总是忠实的自进化者
authors: "Weixiang Zhao, Yingshuo Wang, Yichen Zhang, Yang Deng, Yanyan Zhao, Wanxiang Che, Bing Qin, Ting Liu"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/22ea8d50d4da341efc490ea6f7856457d412c8c7.pdf"
tags: ["query:self-evolve"]
score: 9.0
evidence: 自进化大模型智能体的经验忠实性
tldr: 自进化大语言模型智能体通过积累和复用经验持续改进，但它们是否真正依据这些经验做出决策仍不明确。作者首次系统研究经验忠实性，即智能体决策对给定经验的因果依赖，对原始与浓缩经验施加受控因果干预，覆盖四个代表框架、13个模型骨干和9个环境。结果显示明显不对称：智能体始终依赖原始经验，却常忽视或误读浓缩经验。该工作揭示了自进化智能体经验利用的关键缺陷。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: 自进化LLM智能体依靠积累与复用经验持续改进，但其是否忠实依赖经验来指导行为尚不清楚。
method: 首次系统研究经验忠实性，对原始与浓缩经验施加受控因果干预，评估四个代表框架、13个骨干与9个环境。
result: 发现明显不对称：智能体一致依赖原始经验，却常忽视或误读浓缩经验。
conclusion: 揭示了自进化智能体经验利用的缺陷，为可靠自进化提供重要警示。
---

## Abstract
Self-evolving large language model (LLM) agents continually improve by accumulating and reusing past experience, yet it remains unclear whether they faithfully rely on that experience to guide their behavior. We present the first systematic investigation of \emph{experience faithfulness}—the causal dependence of an agent's decisions on the experience it is given—in self-evolving LLM agents. Using controlled causal interventions on both raw and condensed forms of experience, we comprehensively evaluate four representative frameworks across 13 LLM backbones and 9 environments. Our analysis uncovers a striking asymmetry: while agents consistently depend on raw experience, they often disregard or misinterpret condensed experience, even when it is the only experience provided. This gap persists across single- and multi-agent configurations and across backbone scales. We trace its underlying causes to three factors: the semantic limitations of condensed content, internal processing biases that suppress experience, and task regimes where pretrained priors already suffice. These findings challenge prevailing assumptions about self-evolving methods and underscore the need for more faithful and reliable approaches to experience integration.

---

## 论文详细总结（自动生成）

### 1. 检索相关性
自进化大模型智能体的经验忠实性。

### 2. 核心内容
自进化大语言模型智能体通过积累和复用经验持续改进，但它们是否真正依据这些经验做出决策仍不明确。作者首次系统研究经验忠实性，即智能体决策对给定经验的因果依赖，对原始与浓缩经验施加受控因果干预，覆盖四个代表框架、13个模型骨干和9个环境。结果显示明显不对称：智能体始终依赖原始经验，却常忽视或误读浓缩经验。该工作揭示了自进化智能体经验利用的关键缺陷。

### 3. 对应检索需求
large language model based agents with self-evolution capabilities。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=kTjSSqgqGf](https://openreview.net/forum?id=kTjSSqgqGf)
