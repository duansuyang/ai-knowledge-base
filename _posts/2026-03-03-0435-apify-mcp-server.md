---
title: Apify MCP Server
date: 2026-03-03
time: 04:35
source: GitHub
url: https://github.com/apify/apify-mcp-server
github_url: https://github.com/apify/apify-mcp-server
tags: [Agent, MCP, Data-Extraction, Web-Scraping]
---

# Apify MCP Server

## 1. 项目概述

### 1.1 项目名称
Apify MCP Server

### 1.2 一句话概述
让 AI agents 能够从社交媒体、搜索引擎、电商网站等任何网站提取数据的 MCP 服务器。

### 1.3 详细描述
Apify MCP Server 是 Model Context Protocol 服务器，使 AI agents 能够使用 Apify Store 中数千个现成的爬虫、抓取工具和自动化工具从各种网站提取数据。支持 OAuth 认证，可从 Claude.ai 或 Visual Studio Code 直接使用。

### 1.4 所属领域
- [x] Agent/IAG (智能体、工作流、MCP、Tool Use)
- [ ] LLM/大模型 (预训练、微调、推理、量化)
- [ ] 多模态 (VLM、视频生成、图像生成)
- [ ] 强化学习 (RLHF、GRPO、DPO)
- [ ] 具身智能 (机器人、Sim2Real)
- [x] RAG/知识库 (向量检索、Hybrid Search)
- [ ] AI安全 (对齐、护栏)
- [ ] 训练/部署 (推理引擎、分布式训练)

### 1.5 标签
`#Agent` `#MCP` `#Data-Extraction` `#Web-Scraping`

---

## 2. 项目来源

### 2.1 来源平台
- [x] GitHub

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| 官方网站 | https://mcp.apify.com |
| GitHub仓库 | https://github.com/apify/apify-mcp-server |
| NPM包 | https://www.npmjs.com/package/@apify/actors-mcp-server |

### 2.3 发布时间
- 项目创建: 2025-01-02
- 最近更新: 2026-03-02

### 2.4 作者/团队
Apify 团队

---

## 3. 项目优势

### 3.1 核心创新点

**创新点 1: 标准化 MCP 集成**
- 描述: 将 Apify 的爬虫能力通过 Model Context Protocol 标准集成
- 为什么重要: 允许任何支持 MCP 的 AI 客户端无缝使用网页数据提取能力

**创新点 2: OAuth 支持**
- 描述: 支持 OAuth 认证，简化了客户端连接流程
- 为什么重要: 用户可以直接从 Claude.ai 或 VS Code 使用，无需复杂配置

**创新点 3: 广泛的数据源支持**
- 描述: 支持社交媒体、搜索引擎、地图、电商网站等
- 为什么重要: 覆盖了最常用的数据提取场景

### 3.2 技术优势

| 优势类别 | 具体优势 | 量化指标 |
|---------|---------|---------|
| 易用性 | 一键连接 Claude/VS Code | 无需配置 |
| 功能丰富 | 1000+ 现成爬虫 | 覆盖主流网站 |
| 标准化 | 遵循 MCP 协议 | 跨客户端兼容 |

### 3.3 应用场景

1. **AI 研究**: 为大模型提供实时网页数据
2. **数据收集**: 批量抓取社交媒体/电商数据
3. **市场分析**: 竞品监控和价格追踪
4. **内容聚合**: 从多个来源聚合内容

### 3.4 适用人群

- [x] 研究人员
- [x] 开发者
- [x] 企业/产品经理
- [ ] 学生/学习者

---

## 4. 技术细节

### 4.1 核心方法/架构

#### 4.1.1 MCP 协议集成
基于 Model Context Protocol 标准，通过标准化的接口暴露 Apify 的爬虫能力。

#### 4.1.2 支持的数据源
- 社交媒体: Twitter, LinkedIn, Instagram 等
- 搜索引擎: Google, Bing 等
- 电商: Amazon, eBay, 淘宝等
- 地图: Google Maps, OpenStreetMap 等

### 4.2 技术栈

| 类别 | 技术/工具 |
|------|----------|
| 语言 | TypeScript |
| 协议 | Model Context Protocol (MCP) |
| 认证 | OAuth 2.0 |

---

## 5. 实验流程与结果

### 5.1 性能指标

| 指标 | 数值 |
|------|-----|
| GitHub Stars | 834 |
| Forks | 108 |
| NPM 周下载 | ~10,000+ |

---

## 6. 资源与链接

### 6.1 官方资源

| 资源类型 | 链接 |
|---------|-----|
| 官网 | https://mcp.apify.com |
| GitHub | https://github.com/apify/apify-mcp-server |
| NPM | https://www.npmjs.com/package/@apify/actors-mcp-server |

---

## 7. 总结与评价

### 7.1 项目评分

| 维度 | 评分 | 说明 |
|------|------|-----|
| 创新性 | ⭐⭐⭐⭐ | MCP 协议与爬虫的创新结合 |
| 实用性 | ⭐⭐⭐⭐⭐ | 极高的实用价值 |
| 实验完整性 | ⭐⭐⭐⭐ | 功能完整，文档清晰 |
| 代码质量 | ⭐⭐⭐⭐ | 官方维护，质量有保证 |

### 7.2 综合评价

Apify MCP Server 是一个将传统网页爬虫能力与现代 AI Agent 框架结合的创新项目。通过 MCP 协议，任何 AI 客户端都可以轻松访问丰富的网页数据提取能力。对于需要实时网页数据的 AI 应用来说，这是一个非常实用的工具。

### 7.3 值得关注的点

1. MCP 协议的实际应用案例
2. OAuth 简化认证流程
3. 1000+ 现成爬虫的生态

---

## 8. 附录

### 8.1 更新日志

| 日期 | 更新内容 |
|------|---------|
| 2026-03-02 | 最近更新 |
