---
title: OpenClaw Backup
date: 2026-03-06
time: 14:28
source: GitHub
url: https://github.com/LeoYeAI/openclaw-backup
github_url: https://github.com/LeoYeAI/openclaw-backup
tags: [OpenClaw, Backup, Migration, Tool]
---

# OpenClaw Backup

## 项目概述

### 一句话概述
OpenClaw 实例的一键备份和恢复工具，支持完整数据迁移和跨实例恢复。

### 详细描述
OpenClaw Backup 是一个强大的备份恢复工具，可备份工作区、内存、技能、凭据、Bot Token、API 密钥、Agent 会话历史等全部数据。备份后可在任何新 OpenClaw 实例上零配置恢复，无需重新配对。

### 所属领域
- [x] Agent/IAG (智能体、工作流、MCP、Tool Use)
- [ ] LLM/大模型
- [ ] 多模态
- [ ] 强化学习
- [ ] 具身智能
- [ ] RAG/知识库
- [ ] AI安全
- [ ] 训练/部署

### 标签
`#OpenClaw` `#Backup` `#Migration` `#Tool`

---

## 项目来源

### 来源平台
- [x] GitHub Trending

### 链接
| 链接类型 | URL |
|---------|-----|
| 官方网站 | https://myclaw.ai |
| GitHub仓库 | https://github.com/LeoYeAI/openclaw-backup |
| ClaWHub | https://clawhub.com/skills/myclaw-backup |

### 发布时间
- 创建时间: 2026-03-02
- 发现时间: 2026-03-06

---

## 项目优势

### 核心创新点

#### 创新点 1: 全面备份
- **描述**: 备份所有组件，包括工作区、凭据、会话历史、Cron 任务等
- **为什么重要**: 确保数据完整性和可迁移性
- **对比现有方法**: 之前需要手动备份各组件

#### 创新点 2: 零配置恢复
- **描述**: 恢复后所有渠道自动重连，无需重新配对
- **为什么重要**: 大幅降低迁移成本
- **对比现有方法**: 传统备份需要重新配置所有连接

#### 创新点 3: 浏览器 UI
- **描述**: 提供 Web 界面上传/下载/恢复备份
- **为什么重要**: 简化操作流程
- **对比现有方法**: 纯命令行操作

### 技术优势

| 优势类别 | 具体优势 | 量化指标 |
|---------|---------|---------|
| 完整性 | 全量备份 | 100% |
| 便捷性 | 一键恢复 | 即时 |
| 安全性 | Token保护 | 强制 |

### 应用场景

1. **服务器迁移**: 从旧服务器迁移到新服务器
2. **数据备份**: 定期备份防止数据丢失
3. **实例复制**: 创建多个相同配置的实例

### 适用人群

- [x] 研究人员
- [x] 开发者
- [x] 企业/产品经理
- [ ] 学生/学习者

---

## 技术细节

### 备份内容

| 组件 | 详情 |
|------|------|
| 🧠 Workspace | MEMORY.md, skills, agent files, SOUL.md, USER.md |
| ⚙️ Config | openclaw.json (bot tokens, API keys, model config) |
| 🔑 Credentials | Channel pairing state |
| 📜 Sessions | Full agent conversation history |
| ⏰ Cron jobs | All scheduled tasks |
| 🛡️ Scripts | Guardian, watchdog, start-gateway |

### 使用方法

```bash
# 安装
clawhub install myclaw-backup

# 创建备份
bash scripts/backup.sh /tmp/openclaw-backups

# 恢复 (先 dry-run)
bash scripts/restore.sh openclaw-backup_TIMESTAMP.tar.gz --dry-run
bash scripts/restore.sh openclaw-backup_TIMESTAMP.tar.gz

# 浏览器 UI
bash scripts/serve.sh start --token $(openssl rand -hex 16) --port 7373
```

### 安全特性

- 强制 Token 验证
- 备份文件自动 chmod 600
- 强制 dry-run 确认
- 不暴露到公网

### 技术栈

| 类别 | 技术/工具 |
|------|----------|
| 平台 | OpenClaw / MyClaw.ai |
| 打包 | tar.gz |
| 部署 | ClaWHub |

### 开源相关

| 项目 | 状态 |
|------|-----|
| 开源代码 | [x] 已开源 |
| 开源模型 | [ ] 不适用 |
| 数据集 | [ ] 不适用 |
| API | [ ] 不适用 |

---

## 实验流程与结果

### 局限性分析

#### 已知的局限性

1. **仅支持 OpenClaw**: 不支持其他 AI Agent 平台
2. **敏感数据风险**: 备份包含敏感凭据，需要安全存储

---

## 资源与链接

### 官方资源

| 资源类型 | 链接 |
|---------|-----|
| 官网 | https://myclaw.ai |
| 代码 | https://github.com/LeoYeAI/openclaw-backup |
| ClaWHub | https://clawhub.com/skills/myclaw-backup |

---

## 总结与评价

### 项目评分 (1-5分)

| 维度 | 评分 | 说明 |
|------|------|-----|
| 创新性 | ⭐⭐⭐⭐ | 解决真实需求 |
| 实用性 | ⭐⭐⭐⭐⭐ | 必备工具 |
| 实验完整性 | ⭐⭐⭐⭐ | 功能完整 |
| 代码质量 | ⭐⭐⭐⭐ | 结构清晰 |
| 文档清晰度 | ⭐⭐⭐⭐⭐ | 多语言支持 |

### 综合评价

OpenClaw Backup 是 OpenClaw 生态的重要工具，解决了实例迁移和数据备份的痛点。支持完整备份所有组件，恢复后无需重新配对。提供浏览器 UI 简化操作，安全性也考虑到位。对于运行 OpenClaw 的用户来说，这是必备工具。

### 值得关注的点

1. **全量备份**: 所有组件一键备份
2. **零配置恢复**: 无需重新配对
3. **浏览器 UI**: 简化操作流程
4. **多语言文档**: 支持 7 种语言

### 下一步建议

- **如果你是 OpenClaw 用户**: 立即安装并创建备份
- **如果你是企业**: 将备份加入定期维护计划
