---
title: STRUCTUREDAGENT - Planning with AND/OR Trees
date: 2026-03-06
time: 16:15
source: arXiv
url: https://arxiv.org/abs/2603.05294
paper_url: https://arxiv.org/pdf/2603.05294
tags: [Agent, Planning, WebAgent]
---

# STRUCTUREDAGENT: Planning with AND/OR Trees for Long-Horizon Web Tasks

## 1. 项目概述

### 1.1 一句话概述
提出层次化规划框架，使用动态 AND/OR 树进行高效搜索，结合结构化内存模块跟踪候选解，提升长程 Web 任务性能。

### 1.2 详细描述
现有 Web 智能体在复杂长程任务上表现不佳，原因包括：上下文记忆有限、规划能力弱、贪心行为导致提前终止。STRUCTUREDAGENT 通过层次化规划框架解决这些问题。

### 1.3 所属领域
- [x] Agent/IAG (智能体、工作流、规划)
- [ ] RAG/知识库
- [ ] 其他

### 1.4 标签
`#Agent` `#Planning` `#WebAgent` `#AND-OR-Tree`

---

## 2. 核心创新

### 2.1 动态 AND/OR 树规划
- 使用 AND/OR 树进行搜索空间的高效探索
- 支持层次化分解复杂任务

### 2.2 结构化内存模块
- 跟踪和维护候选解
- 提升信息检索任务的约束满足

### 2.3 可解释性
- 产生可解释的层次化计划
- 便于调试和人工干预

---

## 3. 实验结果

在 WebVoyager、WebArena 和自定义购物基准上测试：
- 显著提升长程 Web 浏览任务性能
- 超越标准 LLM 智能体

---

## 4. 总结

STRUCTUREDAGENT 为 Web 智能体的长程规划提供了新思路，AND/OR 树结构增强了规划的效率和可解释性。

- 论文: https://arxiv.org/abs/2603.05294

*2026-03-06*
