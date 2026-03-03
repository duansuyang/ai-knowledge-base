---
title: MobilityBench - LLM路径规划Agent评估基准
date: 2026-03-03
time: 20:27
source: GitHub/PaperswithCode
url: https://github.com/AMAP-ML/MobilityBench
paper_url: https://arxiv.org/abs/2602.22638
github_url: https://github.com/AMAP-ML/MobilityBench
tags: [Agent, 评估基准, 路径规划, LLM]
---

# MobilityBench - LLM路径规划Agent评估基准

## 1. 项目概述

### 1.1 项目名称
MobilityBench

### 1.2 一句话概述
阿里巴巴高德发布的LLM路径规划Agent评估基准，基于大规模真实用户查询构建，支持可复现的端到端评估。

### 1.3 详细描述
MobilityBench是首个规模化评估LLM路径规划Agent的基准数据集，基于高德地图大规模匿名用户查询构建，覆盖22个国家350+城市。它提供确定性API重放沙箱，支持结果可复现评估，并引入多维度评估协议。

### 1.4 所属领域
- [x] Agent/IAG (智能体、工作流、MCP、Tool Use)
- [ ] LLM/大模型 (预训练、微调、推理、量化)
- [ ] 评估基准 (Benchmark)
- [ ] 具身智能 (机器人、Sim2Real)

### 1.5 标签
`#Agent` `#评估基准` `#路径规划` `#LLM` `#地图`

---

## 2. 项目来源

### 2.1 来源平台
- [x] arXiv 论文
- [x] GitHub Trending
- [x] Hugging Face
- [x] Papers with Code

### 2.2 链接

| 链接类型 | URL |
|---------|-----|
| 官方网站 | https://github.com/AMAP-ML/MobilityBench |
| 论文PDF | https://arxiv.org/abs/2602.22638 |
| GitHub仓库 | https://github.com/AMAP-ML/MobilityBench |
| 数据集 | https://huggingface.co/datasets/GD-ML/MobilityBench |

### 2.3 发布时间
- 论文/项目发布日期: 2026-02-26
- 发现日期: 2026-03-03

### 2.4 作者/团队

| 成员 | 机构/职位 |
|------|----------|
| Zhiheng Song | 高德 (AMAP, Alibaba) |
| Jingshuai Zhang | 高德 (AMAP, Alibaba) |
| Chuan Qin | 高德 (AMAP, Alibaba) |
| Chao Wang | 高德 |
| Longfei Xu | 高德 |
| Kaikui Liu | 高德 |
| Xiangxiang Chu | 高德 |
| Hengshu Zhu | 高德 (Corresponding) |

---

## 3. 项目优势

### 3.1 核心创新点

#### 创新点 1: 大规模真实数据
- **描述**: 基于高德地图100,000条真实用户路径规划查询构建
- **为什么重要**: 填补了LLM路径规划评估的空白
- **对比现有方法**: 之前没有专门针对路径规划的Agent基准

#### 创新点 2: 确定性API重放沙箱
- **描述**: 提供确定性API-replay sandbox，消除环境差异
- **为什么重要**: 支持可复现的端到端评估
- **对比现有方法**: 之前依赖在线服务，评估结果不稳定

#### 创新点 3: 多维度评估协议
- **描述**: 以结果有效性为核心，辅以指令理解、规划、工具使用和效率评估
- **为什么重要**: 全面评估Agent能力
- **对比现有方法**: 单一指标无法反映Agent综合能力

### 3.2 数据规模

| 维度 | 数据 |
|------|------|
| 样本数量 | 100,000 episodes |
| 覆盖国家 | 22 |
| 覆盖城市 | 350+ |
| 任务类型 | 11种意图 |

### 3.3 任务分布

| 意图类型 | 占比 |
|---------|------|
| 基本路线规划 | 42.5% |
| 基本信息检索 | 36.6% |
| 偏好约束路线规划 | 11.3% |
| 路线相关信息检索 | 9.6% |

### 3.4 应用场景

1. **评估LLM路径规划能力**: 评估Agent在真实地图场景下的表现
2. **Agent框架对比**: 比较Plan-and-Execute vs ReAct
3. **模型选择**: 为产品选择合适的LLM后端
4. **模型改进**: 发现Agent能力的不足

### 3.5 适用人群

- [x] 研究人员
- [x] 开发者
- [x] 企业/产品经理
- [ ] 学生/学习者

---

## 4. 技术细节

### 4.1 支持的Agent框架

#### Plan-and-Execute (默认)
- **Planner**: 分析需求，创建结构化计划
- **Worker**: 执行工具调用
- **Reporter**: 生成自然语言报告

#### ReAct
- **Reasoning**: 分析当前状态
- **Action**: 执行工具调用
- **Observation**: 处理工具结果

### 4.2 支持的模型

| 模型 | 厂商 |
|------|------|
| GPT-5.2 | OpenAI |
| GPT-4.1 | OpenAI |
| Claude-Opus-4.5 | Anthropic |
| Claude-Sonnet-4.5 | Anthropic |
| Gemini-3-Flash/Pro | Google |
| DeepSeek-V3.2-Exp | DeepSeek |
| DeepSeek-R1 | DeepSeek |
| Qwen3-4B/30B/32B/235B | Alibaba |

### 4.3 技术栈

| 类别 | 技术/工具 |
|------|----------|
| 框架 | LangGraph |
| CLI | Python (uv) |
| 评估 | 多维度评估协议 |
| 沙箱 | 确定性API重放 |

### 4.4 开源相关

| 项目 | 状态 |
|------|-----|
| 开源代码 | ✅ 已开源 |
| 开源数据集 | ✅ 已发布 (HuggingFace) |
| 预训练模型 | ❌ 未发布 |
| API | ❌ 未提供 |

---

## 5. 数据格式

### 5.1 数据字段

| 字段 | 说明 |
|------|------|
| query | 用户查询文本 |
| context | 上下文信息 (JSON) |
| task_scenario | 细粒度任务类别 |
| intent_family | 粗粒度意图类别 |
| tool_list | 预期工具调用 |
| route_ans | 真实路线答案 (JSON) |

### 5.2 示例

```
Query: "去大石桥不走高速"
Task Scenario: Option-Constrained Route Planning
Intent Family: Preference-Constrained Route Planning
```

---

## 6. 使用方法

### 6.1 安装

```bash
git clone https://github.com/AMAP-ML/MobilityBench.git
cd MobilityBench
uv sync  # or pip install -e .
```

### 6.2 运行评估

```bash
# 使用默认配置运行
mbench run --model gpt4.1 --dataset data/datasets/sample_10.csv

# 使用ReAct框架
mbench run --model gpt4.1 --framework react

# 评估结果
mbench eval --run-id run_xxx
```

---

## 7. 总结与评价

### 7.1 项目评分

| 维度 | 评分 | 说明 |
|------|------|-----|
| 创新性 | ⭐⭐⭐⭐⭐ | 首个路径规划Agent基准 |
| 实用性 | ⭐⭐⭐⭐⭐ | 真实数据+可复现评估 |
| 实验完整性 | ⭐⭐⭐⭐⭐ | 完整工具链 |
| 代码质量 | ⭐⭐⭐⭐ | 文档完善 |

### 7.2 综合评价

MobilityBench是LLM Agent评估领域的重要贡献，首次大规模系统性地评估LLM在路径规划场景下的能力。数据集来自真实用户需求，评估协议科学严谨，沙箱设计确保可复现性。对做Agent研究的团队有重要参考价值。

### 7.3 值得关注的点

1. 100,000条真实用户查询，数据规模大
2. 确定性API重放沙箱，支持离线评估
3. 多维度评估协议，全面反映Agent能力
4. 支持主流LLM和两种Agent框架

---

## 8. 附录

### 8.1 更新日志

| 日期 | 更新内容 |
|------|---------|
| 2026-02-26 | 首次发布 |
| 2026-03-02 | 最新提交 |
