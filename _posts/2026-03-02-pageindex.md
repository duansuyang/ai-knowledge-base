---
title: PageIndex - 向量无关的推理型 RAG
date: 2026-03-02
time: 00:21
source: GitHub
url: https://github.com/vectifyai/PageIndex
github_url: https://github.com/vectifyai/PageIndex
tags: [RAG, Agent, Reasoning, LLM]
---

# PageIndex: 向量无关的推理型 RAG

## 1. 项目概述

### 1.1 一句话概述
PageIndex 是一个无需向量数据库、无需分块的推理型 RAG 框架，通过构建文档的树形索引结构，让 LLM 像人类专家一样推理检索专业长文档。

### 1.2 详细描述
传统基于向量的 RAG 依赖语义"相似度"而非真正"相关性"。PageIndex 受 AlphaGo 启发，提出基于树搜索的推理检索方法：先将文档解析为树形结构索引，再让 LLM 在索引上进行推理导航，模拟人类阅读专业文档的方式。

### 1.3 所属领域
- [x] RAG/知识库 (向量检索、Hybrid Search)
- [x] Agent/IAG (智能体、工作流)

---

## 2. 项目来源

### 2.1 来源平台
- [x] GitHub Trending

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| GitHub | https://github.com/vectifyai/PageIndex |
| 官网 | https://vectify.ai/pageindex |
| 文档 | https://docs.pageindex.ai |
| 在线演示 | https://chat.pageindex.ai |

### 2.3 关键数据
- **Stars**: 19,575
- **Forks**: 1,458
- **创建时间**: 2025-04-01

---

## 3. 核心创新

### 3.1 三大核心特性
| 特性 | 说明 |
|------|-----|
| 无需向量数据库 | 使用文档结构 + LLM 推理进行检索 |
| 无需分块 | 文档按自然章节组织，非人工切分 |
| 类人检索 | 模拟人类专家导航和提取知识的方式 |

### 3.2 技术原理
1. **构建树形索引**: 将长文档解析为类似"目录"的树结构
2. **推理检索**: LLM 在树结构上进行树搜索，推理导航到相关章节

### 3.3 性能表现
- **FinanceBench 准确率**: 98.7%（SOTA）
- 显著优于传统向量 RAG 方案

---

## 4. 应用场景

1. **金融报表分析**: 解析年报、招股书、监管文件
2. **法律文档检索**: 合同、判例、法规
3. **学术论文理解**: 教科书、论文全文
4. **技术文档问答**: API 文档、架构说明

---

## 5. 部署方式

- **自托管**: 开源仓库本地运行
- **云服务**: Chat 平台直接使用
- **MCP 集成**: 支持 Claude、Cursor 等 AI 助手
- **API**: 提供 REST API

---

## 6. 总结

**创新性**: ⭐⭐⭐⭐⭐ 首次提出向量无关的推理检索范式
**实用性**: ⭐⭐⭐⭐⭐ 已在金融文档分析取得 SOTA 效果
**代码质量**: ⭐⭐⭐⭐ 开源完整，提供 Cookbook

**适合人群**: RAG 开发者、企业知识库工程师、AI 应用研究者

**链接**: https://github.com/vectifyai/PageIndex
