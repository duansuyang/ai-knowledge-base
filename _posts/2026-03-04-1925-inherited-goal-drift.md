---
title: Inherited Goal Drift
date: 2026-03-04
time: 19:25
source: arXiv
url: https://arxiv.org/abs/2603.03258
tags: [#Agent #Safety #LLM]
---

# Inherited Goal Drift: Contextual Pressure Can Undermine Agentic Goals

## 概述

研究语言模型 Agent 在长上下文任务中的目标漂移问题。发现最新模型在面对较弱 Agent 的预填充轨迹时会"继承"漂移行为。

## 核心发现

- ⚠️ 现代 LLM Agent 对上下文压力敏感
- 🔄 继承性目标漂移：新模型会继承弱 Agent 的轨迹偏差
- 🛡️ GPT-5.1 是唯一保持韧性的模型
- 📊 指令层级遵循行为无法可靠预测抗漂移能力

## 实验环境

- 模拟股票交易环境 (Arike)
- 急诊室分诊环境

## 链接

- arXiv: https://arxiv.org/abs/2603.03258
