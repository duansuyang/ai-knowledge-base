---
title: OpenClaw Guardian
date: 2026-03-03
time: 07:05
source: GitHub
url: https://github.com/LeoYeAI/openclaw-guardian
github_url: https://github.com/LeoYeAI/openclaw-guardian
tags: ["OpenClaw", "Guardian", "Monitor", "DevOps", "Agent"]
---

# OpenClaw Guardian

## 1. 项目概述

### 1.1 项目名称
OpenClaw Guardian

### 1.2 一句话概述
OpenClaw Gateway的守护者 watchdog，实现自动监控、自愈修复和Git回滚。

### 1.3 详细描述
OpenClaw Guardian是MyClaw.ai生产基础设施的硬化层，专为7x24小时运行的AI Agent实例设计。每30秒检查Gateway健康状态，失败时自动运行修复命令，支持Git回滚和Discord告警。

### 1.4 所属领域
- [x] Agent/IAG (智能体、工作流、MCP、Tool Use)
- [x] 训练/部署 (推理引擎、分布式训练)
- [ ] 其他: ________

### 1.5 标签
`#OpenClaw` `#Guardian` `#Monitor` `#DevOps` `#Auto-Repair`

---

## 2. 项目来源

### 2.1 来源平台
- [x] GitHub

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| GitHub仓库 | https://github.com/LeoYeAI/openclaw-guardian |
| MyClaw.ai | https://myclaw.ai |

### 2.3 发布时间
- 发布日期: 2026-03-02
- 发现日期: 2026-03-03

### 2.4 作者/团队
| 成员 | 机构/职位 |
|------|----------|
| LeoYeAI | MyClaw.ai |

---

## 3. 项目优势

### 3.1 核心创新点

#### 创新点 1: 自愈机制
- **描述**: 检测到Gateway故障时，自动运行`openclaw doctor --fix`进行修复，最多尝试3次
- **为什么重要**: AI Agent通常需要7x24小时运行，故障自动恢复至关重要
- **对比现有方法**: 传统方法需要人工干预，该项目实现全自动化

#### 创新点 2: Git回滚
- **描述**: 修复失败时自动回滚到上一个稳定的Git提交
- **为什么重要**: 确保系统始终处于可预测的稳定状态
- **对比现有方法**: 配合自愈机制，提供双重保障

#### 创新点 3: 每日快照
- **描述**: 每日自动Git提交工作区变化
- **为什么重要**: 保留完整的变更历史，便于追踪和回滚

### 3.2 技术优势

| 优势类别 | 具体优势 | 量化指标 |
|---------|---------|---------|
| 监控频率 | 30秒检查间隔 | 实时 |
| 修复能力 | 最多3次自愈尝试 | 自动化 |
| 告警支持 | Discord Webhook | 即时通知 |
| 易用性 | AI Agent一键安装 | 零配置 |

---

## 4. 总结与评价

### 4.1 项目评分

| 维度 | 评分 | 说明 |
|------|------|-----|
| 创新性 | ⭐⭐⭐⭐⭐ | Agent运维自动化 |
| 实用性 | ⭐⭐⭐⭐⭐ | 生产级可用 |
| 实验完整性 | ⭐⭐⭐⭐ | 功能完整 |
| 代码质量 | ⭐⭐⭐⭐ | Shell脚本 |

### 4.2 综合评价

OpenClaw Guardian是AI Agent运维的重要工具，解决了生产环境中7x24小时运行的关键问题。自愈、Git回滚、每日快照等功能形成了一套完整的保障体系。

### 4.3 值得关注的点

1. 自动健康检查机制
2. Git-based回滚策略
3. Discord告警集成

### 4.4 下一步建议

- **如果你是OpenClaw用户**: 立即安装以保护你的Gateway
- **如果你是运维工程师**: 将此工具纳入AI Agent部署方案

---

## 5. 更新日志

| 日期 | 更新内容 |
|------|---------|
| 2026-03-03 | 首次创建 |
