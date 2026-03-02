---
title: MobilityBench
date: 2026-03-02
time: 18:36
source: HuggingFace Papers
url: https://huggingface.co/papers/2602.22638
paper_url: https://arxiv.org/abs/2602.22638
github_url: https://github.com/AMAP-ML/MobilityBench
tags: [Agent, Benchmark, LLM, Route-Planning]
---

# MobilityBench: A Benchmark for Evaluating Route-Planning Agents in Real-World Mobility Scenarios

## 1. 项目概述

### 1.1 项目名称
MobilityBench

### 1.2 一句话概述
阿里巴巴发布的大规模LLM路线规划智能体评估基准，基于高德真实用户查询构建。

### 1.3 详细描述
MobilityBench是一个可扩展的评估基准，用于在真实移动场景中评估基于LLM的路线规划智能体。该基准来自高德地图大规模匿名真实用户查询，覆盖全球多个城市的各类路线规划意图。

### 1.4 所属领域
- [x] Agent/IAG (智能体、工作流、MCP、Tool Use)
- [ ] LLM/大模型 (预训练、微调、推理、量化)
- [ ] 多模态 (VLM、视频生成、图像生成)
- [ ] 强化学习 (RLHF、GRPO、DPO)
- [ ] 具身智能 (机器人、Sim2Real)
- [ ] RAG/知识库 (向量检索、Hybrid Search)
- [ ] AI安全 (对齐、护栏)
- [ ] 训练/部署 (推理引擎、分布式训练)

### 1.5 标签
`#Agent` `#Benchmark` `#LLM` `#Route-Planning`

---

## 2. 项目来源

### 2.1 来源平台
- [x] arXiv 论文
- [ ] GitHubTrending
- [ ] Hugging Face
- [ ] Papers with Code

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| 官方网站 | https://huggingface.co/papers/2602.22638 |
| 论文PDF | https://arxiv.org/pdf/2602.22638 |
| GitHub仓库 | https://github.com/AMAP-ML/MobilityBench |
| Demo演示 | - |
| HuggingFace | https://huggingface.co/papers/2602.22638 |

### 2.3 发布时间
- 论文/项目发布日期: 2026-02-26
- 发现日期: 2026-03-02

### 2.4 作者/团队
| 成员 | 机构/职位 |
|------|----------|
| Zhiheng Song | Alibaba |
| Jingshuai Zhang | Alibaba |
| Chao Wang | Alibaba |
| Longfei Xu | Alibaba |
| Xiangxiang Chu | Alibaba |
| Hengshu Zhu | Alibaba |

---

## 3. 项目优势

### 3.1 核心创新点

#### 创新点 1: 大规模真实用户数据
- **描述**: 基于高德地图大规模匿名真实用户查询构建
- **为什么重要**: 解决了现有基准缺乏真实性的问题
- **对比现有方法**: 比合成数据更贴近实际应用场景

#### 创新点 2: 确定性的API重放沙箱
- **描述**: 设计了确定性的API重放沙箱，消除环境差异
- **为什么重要**: 实现可复现的端到端评估
- **对比现有方法**: 解决了线上地图服务非确定性问题

#### 创新点 3: 多维评估协议
- **描述**: 以结果有效性为中心，辅以指令理解、规划、工具使用和效率评估
- **为什么重要**: 全面评估智能体能力
- **对比现有方法**: 比单一指标更全面

### 3.2 实验发现

**关键发现**: 当前模型在基础信息检索和路线规划任务上表现良好，但在偏好约束路线规划任务上表现困难，说明个性化移动应用仍有很大改进空间。

---

## 4. 资源与链接

### 4.1 官方资源
| 资源类型 | 链接 |
|---------|-----|
| 论文 | https://arxiv.org/abs/2602.22638 |
| 代码 | https://github.com/AMAP-ML/MobilityBench |
| 数据集 | https://huggingface.co/datasets/GD-ML/MobilityBench |

---

## 5. 总结与评价

### 5.1 项目评分
| 维度 | 评分 |
|------|------|
| 创新性 | ⭐⭐⭐⭐ |
| 实用性 | ⭐⭐⭐⭐⭐ |
| 实验完整性 | ⭐⭐⭐⭐⭐ |

### 5.2 综合评价
MobilityBench是首个大规模评估LLM路线规划智能体的基准，对于推动智能体在实际场景中的应用具有重要意义。阿里巴巴开源了基准数据和评估工具，值得关注。
