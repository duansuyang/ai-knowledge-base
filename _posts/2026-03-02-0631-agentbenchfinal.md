---
title: Qwen2.5-7B AgentBench Fine-tuned Model
date: 2026-03-02
time: 06:31
source: HuggingFace
url: https://huggingface.co/takayosh/agentbenchfinal
tags: [Agent, Qwen2.5, Tool-Use, ALFWorld, DBBench]
---

# Qwen2.5-7B AgentBench Fine-tuned Model

## 项目概述

基于 Qwen2.5-7B-Instruct 的Agent模型，针对ALFWorld和DBBench任务进行了微调优化。

## 核心特性

- **模型架构**: Qwen2.5-7B-Instruct + LoRA adapters
- **训练数据**: ALFWorld轨迹数据 + DBBench ReAct数据集
- **合并方法**: TIES merge (density=0.1)
- **工具使用**: 支持ALFWorld和DBBench评估环境

## 技术细节

训练流程:
1. 在ALFWorld上训练LoRA适配器
2. 在DBBench上训练LoRA适配器
3. 使用TIES方法合并适配器 (density=0.1)
4. 进行额外稳定化微调
5. 最终合并到基础模型

## 适用场景

- Agent评估基准测试
- 工具调用任务
- 多步骤推理任务

## 相关链接

- HuggingFace: https://huggingface.co/takayosh/agentbenchfinal
- 基础模型: Qwen/Qwen2.5-7B-Instruct
