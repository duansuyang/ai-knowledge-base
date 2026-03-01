---
title: LittleMonster Reasoning 12B - Heretic Decensored
date: 2026-03-02
time: 06:31
source: HuggingFace
url: https://huggingface.co/reedmayhew/littlemonster-reasoning-12B-QKVO-hereticv2-HF
tags: [Reasoning, Gemma3, Uncensored, Unsloth]
---

# LittleMonster Reasoning 12B - Heretic Decensored

## 项目概述

基于Gemma-3 12B的去审查化(Decensored)推理模型，使用Heretic技术进行去审查化处理。

## 核心特性

- **基础模型**: google/gemma-3-12b-it
- **去审查化方法**: Heretic v1.2.0
- **训练框架**: Unsloth + TRL
- **参数规模**: 12B

## 技术细节

Abliteration参数:
- attention o_proj max_weight: 1.34
- mlp down_proj max_weight: 0.87

性能对比:
| 模型 | 拒绝率 (Refusals) |
|------|------------------|
| Decensored版本 | 47/100 |
| 原始版本 | 78/100 |

## 适用场景

- 需要较少限制的推理任务
- 创意写作
- 代码生成

## 相关链接

- HuggingFace: https://huggingface.co/reedmayhew/littlemonster-reasoning-12B-QKVO-hereticv2-HF
- Heretic工具: https://github.com/p-e-w/heretic
- Unsloth: https://github.com/unslothai/unsloth
