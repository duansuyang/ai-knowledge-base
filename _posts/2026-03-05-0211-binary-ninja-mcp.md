---
title: Binary Ninja Headless MCP
date: 2026-03-05
time: 02:11
source: GitHub
url: https://github.com/mrphrazer/binary-ninja-headless-mcp
github_url: https://github.com/mrphrazer/binary-ninja-headless-mcp
tags: [MCP, Agent, Security, ReverseEngineering]
---

# Binary Ninja Headless MCP

## 1. 项目概述

### 1.1 项目名称
Binary Ninja Headless MCP

### 1.2 一句话概述
支持AI智能体进行深度逆向工程的MCP服务器，提供180+工具函数。

### 1.3 详细描述
一个Headless Binary Ninja服务器，通过MCP协议为AI智能体提供完整的逆向工程工作流访问——包括反汇编、IL、补丁、类型、xref等，无需GUI。

### 1.4 所属领域
- [x] Agent/IAG (智能体、工作流、MCP、Tool Use)
- [x] AI安全 (对齐、护栏)

### 1.5 标签
`#MCP` `#Agent` `#Security` `#ReverseEngineering`

---

## 2. 项目来源

### 2.1 来源平台
- [x] GitHubTrending

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| 官方网站 | https://github.com/mrphrazer/binary-ninja-headless-mcp |
| GitHub仓库 | https://github.com/mrphrazer/binary-ninja-headless-mcp |

### 2.3 发布时间
- 发布日期: 2026-03-03
- 发现日期: 2026-03-05

### 2.4 作者/团队
| 成员 | 机构/职位 |
|------|----------|
| mrphrazer | 安全研究员 |

---

## 3. 项目优势

### 3.1 核心创新点

#### 创新点 1: 纯Headless设计
- **描述**: 专为沙箱VM/容器环境中的智能体驱动工作流设计，无需GUI
- **为什么重要**: 现有Binary Ninja MCP服务器都依赖GUI或功能受限
- **对比现有方法**: 完整的功能覆盖，180+工具函数

#### 创新点 2: 安全 mutation 工作流
- **描述**: 默认只读，支持undo/redo和事务
- **为什么重要**: 确保逆向工程过程可回滚，安全可控
- **对比现有方法**: 提供企业级的安全保障

#### 创新点 3: 脚本访问能力
- **描述**: 通过binja.eval和binja.call访问工具目录未覆盖的功能
- **为什么重要**: 高度可扩展
- **对比现有方法**: 比现有方案更灵活

### 3.2 技术优势

| 优势类别 | 具体优势 | 量化指标 |
|---------|---------|---------|
| 功能丰富 | 工具函数数量 | 180+ |
| 功能分组 | 特性组数量 | 35 |
| 灵活性 | 支持stdio和TCP传输 | 是 |
| 可扩展性 | 脚本访问 | 是 |

### 3.3 应用场景

1. **自动化逆向工程**: 智能体可自主分析二进制文件
2. **恶意软件分析**: 安全研究自动化
3. **漏洞挖掘**: 大规模二进制分析

### 3.4 适用人群
- [x] 研究人员 (安全研究员)
- [x] 开发者
- [x] 企业/产品经理

---

## 4. 技术细节

### 4.1 核心功能

支持180+工具函数，覆盖：
- 分析 (Analysis)
- 反汇编 (Disassembly)
- IL (Intermediate Language)
- 补丁 (Patching)
- Undo/Redo
- 类型 (Types)
- 工作流 (Workflows)
- 内存 (Memory)
- 搜索 (Search)
- XRefs
- 脚本 (Scripting)

### 4.2 系统要求

| 组件 | 要求 |
|------|-----|
| Python | 3.11+ |
| Binary Ninja | 需要headless-capable license |
| 运行环境 | Docker容器 |

### 4.3 传输方式

- Stdio
- TCP
- Fake backend模式 (CI/开发无需license)

### 4.4 开源相关

| 项目 | 状态 |
|------|-----|
| 开源代码 | [x] 已开源 |
| 开源模型 | N/A |
| 数据集 | N/A |

---

## 5. 总结与评价

### 5.1 项目评分

| 维度 | 评分 | 说明 |
|------|------|-----|
| 创新性 | ⭐⭐⭐⭐ | 垂直领域创新 |
| 实用性 | ⭐⭐⭐⭐ | 解决实际问题 |
| 实验完整性 | ⭐⭐⭐ | 项目原型 |

### 5.2 综合评价

Binary Ninja Headless MCP是首个真正为AI智能体设计的headless逆向工程MCP服务器。它让智能体可以完全控制分析系统，自动化大部分逆向工程工作流。这是一个非常垂直但有价值的技术突破。

### 5.3 值得关注的点

1. 180+工具函数覆盖逆向工程全流程
2. 默认只读+安全mutation设计
3. 支持fake backend模式便于开发

---

## 6. 更新日志

| 日期 | 更新内容 |
|------|---------|
| 2026-03-05 | 首次创建 |
