---
title: Memory-Like-A-Tree
date: 2026-03-02
time: 07:31
source: GitHub
url: https://github.com/loryoncloud/Memory-Like-A-Tree
github_url: https://github.com/loryoncloud/Memory-Like-A-Tree
tags: [Agent, Memory, Knowledge-Management]
---

# Memory-Like-A-Tree 🌳

## 项目概述

为 AI Agent 设计的记忆管理系统，让知识像树一样生长。核心理念：Agent 正常工作，树自动生长。

## 核心概念

- 🌱 新知识像种子一样萌芽 (置信度 0.7)
- 🌿 常用的知识茁壮成长 (置信度 >= 0.8)
- 🍂 不用的知识自然凋零 (置信度 0.5-0.8)
- 🪨 落叶化作养分，滋养新的生长

## 架构组件

- **indexer** - 索引新知识
- **search** - 语义搜索
- **confidence-db** - 置信度追踪
- **decayer** - 每天自动衰减置信度
- **cleaner** - 清理低置信度知识，提取精华

## 特性

- 置信度生命周期管理
- 自动衰减机制
- 跨 Agent 搜索
- Obsidian 同步
