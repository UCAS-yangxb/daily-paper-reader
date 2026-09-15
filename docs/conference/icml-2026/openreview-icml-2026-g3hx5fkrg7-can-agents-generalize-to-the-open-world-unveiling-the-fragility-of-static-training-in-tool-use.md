---
title: Can Agents Generalize to the Open World? Unveiling the Fragility of Static Training in Tool Use
title_zh: 智能体能否泛化到开放世界？揭示工具使用中静态训练的脆弱性
authors: "Weiming Wu, Song-Lin Lv, Rui Zhu, Zi-Jian Cheng, Lan-Zhe Guo"
date: 2026
publication_date: 2026
publication_date_precision: year
publication_date_source: conference year only; exact release date unverified
publication_date_kind: unknown
pdf: "https://openreview.net/pdf/b6f9c98cff9e43b831a4aed668c0e4b0024a1a05.pdf"
tags: ["query:self-evolve"]
score: 5.0
evidence: 工具智能体适应动态开放世界
tldr: 大模型智能体虽在静态基准表现优异，却难以应对真实世界动态变化的查询、工具集与交互。本文形式化OpenAgent开放世界工具使用设定，构建受控沙箱并定义感知、交互、推理、内化四层环境偏移。系统实验揭示静态训练在分布偏移下的脆弱性，为开放世界智能体泛化诊断提供基准。
source: ICML-2026-Accepted
selection_source: conference_retrieval
motivation: LLM智能体在静态基准表现良好，却难以应对真实世界动态查询与工具集。
method: 形式化OpenAgent开放世界工具使用设定，构建受控沙箱与四层环境偏移层级。
result: 系统实验揭示静态训练在分布偏移下的脆弱性。
conclusion: 为开放世界智能体泛化提供诊断基准与洞见。
---

## Abstract
While Large Language Model (LLM) agents demonstrate proficiency in static benchmarks, their deployment in real-world scenarios is hindered by the dynamic nature of user queries, tool sets, and interaction dynamics.To address this generalization gap, we formalize **OpenAgent** (Tool-Use Agent in Open-World), a problem setting characterized by distributional shifts across query, action, observation, and domain dimensions.To systematically diagnose its impact, we construct a controlled sandbox environment where we define fine-grained environmental shifts across a four-tier hierarchy, *Perception*, *Interaction*, *Reasoning*, and *Internalization*, and conduct a comprehensive series of experiments. Our analysis yields a series of key insights, demonstrating that agents trained via both Supervised Fine-Tuning (SFT) and Reinforcement Learning suffer from varying degrees of performance degradation when confronting open environmental shifts.Building on these insights, we propose Perturbation-Augmented Fine-Tuning, a disturbance-based intervention strategy for SFT that lays the foundation for enhancing agent robustness and utility in realistic environments. Our code will be released at: [https://github.com/LAMDA-NeSy/OpenAgent](https://github.com/LAMDA-NeSy/OpenAgent).

---

## 论文详细总结（自动生成）

### 1. 检索相关性
工具智能体适应动态开放世界。

### 2. 核心内容
大模型智能体虽在静态基准表现优异，却难以应对真实世界动态变化的查询、工具集与交互。本文形式化OpenAgent开放世界工具使用设定，构建受控沙箱并定义感知、交互、推理、内化四层环境偏移。系统实验揭示静态训练在分布偏移下的脆弱性，为开放世界智能体泛化诊断提供基准。

### 3. 对应检索需求
adaptive mechanisms enabling agents to evolve in dynamic environments。

### 4. 来源与原文
- Source：ICML-2026-Accepted
- OpenReview：[https://openreview.net/forum?id=G3hX5Fkrg7](https://openreview.net/forum?id=G3hX5Fkrg7)
