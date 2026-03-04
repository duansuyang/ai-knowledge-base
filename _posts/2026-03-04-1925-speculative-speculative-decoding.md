---
title: Speculative Speculative Decoding
date: 2026-03-04
time: 19:25
source: arXiv
url: https://arxiv.org/abs/2603.03251
tags: [#LLM #Inference #Optimization]
---

# Speculative Speculative Decoding

## 概述

提出 Speculative Speculative Decoding (SSD)，将推测解码的推测和验证操作并行化，进一步加速 LLM 推理。

## 核心创新

- ⚡ 并行化推测与验证
- 🎯 预测验证结果并预先准备推测
- 🚀 Saguaro 实现：比优化后的推测解码快 2x，比自回归解码快 5x

## 技术细节

- 解决三个关键挑战
- 验证期间草案模型预测可能的验证结果
- 如果实际验证结果在预测集中，可立即返回推测

## 链接

- arXiv: https://arxiv.org/abs/2603.03251
