---
title: Anthropic Agent Skills
date: 2026-03-04
time: 21:25
source: GitHub
url: https://github.com/anthropics/skills
github_url: https://github.com/anthropics/skills
tags: [#Agent, #Skills, #Anthropic, #Claude]
---

# Anthropic Agent Skills

## 1. 项目概述

### 1.1 项目名称
Anthropic Agent Skills

### 1.2 一句话概述
Anthropic 公开的 Claude Agent Skills 仓库，包含用于各种专业任务的动态加载技能集合。

### 1.3 详细描述
该仓库包含 Claude 用于完成专业任务的指令、脚本和资源集合。Skills 教会 Claude 如何以可重复的方式完成特定任务，包括创建符合公司品牌指南的文档、使用组织特定工作流程分析数据，或自动化个人任务。

### 1.4 所属领域
- [x] Agent/IAG (智能体、工作流、MCP、Tool Use)

### 1.5 标签
`#Agent` `#Skills` `#Anthropic` `#Claude`

---

## 2. 项目来源

### 2.1 来源平台
- [x] GitHubTrending

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| 官方网站 | https://github.com/anthropics/skills |
| 文档 | https://support.claude.com/en/articles/12512176-what-are-skills |
| Agent Skills 标准 | https://agentskills.io |

### 2.3 发布时间
- 发布日期: 2026年
- 发现日期: 2026-03-04

---

## 3. 项目优势

### 3.1 核心创新点

#### 创新点 1: 标准化 Agent Skills 架构
- **描述**: 定义了 SKILL.md 格式，包含 YAML frontmatter 和指令，使 AI 能够动态加载专业技能
- **为什么重要**: 让 AI 能够像人类一样"学习"专业领域的知识和工作流程

#### 创新点 2: 开源技能集合
- **描述**: 公开了用于创意设计、开发技术、企业通信和文档处理的完整技能示例
- **为什么重要**: 为开发者提供了创建自定义技能的参考实现

### 3.2 技术优势

| 优势类别 | 具体优势 |
|---------|---------|
| 可扩展性 | 支持自定义 Skills，可动态加载 |
| 多平台支持 | Claude Code、Claude.ai、API 都支持 |
| 开源示例 | 包含 Apache 2.0 许可的开源技能 |

### 3.3 应用场景

1. **企业工作流自动化**: 创建符合公司品牌指南的文档
2. **数据分析**: 使用组织特定工作流程分析数据
3. **个人任务自动化**: 自动化重复性个人任务

### 3.4 适用人群

- [x] 开发者
- [x] 企业/产品经理
- [x] 研究人员

---

## 4. 技术细节

### 4.1 核心方法

Skills 是包含指令、脚本和资源的文件夹，Claude 可以动态加载这些内容来提高专业任务的性能。每个 skill 都是自包含的，有自己的 `SKILL.md` 文件。

### 4.2 Skill 格式

```markdown
---
name: my-skill-name
description: A clear description of what this skill does
---

# My Skill Name

[Add instructions here]

## Examples
- Example usage 1
- Example usage 2
```

### 4.3 开源相关

| 项目 | 状态 |
|------|-----|
| 开源代码 | [x] 已开源 (Apache 2.0) |
| 文档 | [x] 已公开 |

---

## 5. 总结与评价

### 5.1 项目评分 (1-5分)

| 维度 | 评分 | 说明 |
|------|------|-----|
| 创新性 | ⭐⭐⭐⭐⭐ | 标准化了 Agent Skills 架构 |
| 实用性 | ⭐⭐⭐⭐⭐ | 开箱即用的多种技能 |
| 实验完整性 | ⭐⭐⭐⭐ | 文档完善 |
| 代码质量 | ⭐⭐⭐⭐⭐ | Anthropic 官方维护 |

### 5.2 综合评价

Anthropic 公开的 Agent Skills 仓库是 AI Agent 领域的重要里程碑。它不仅提供了标准化的技能定义格式，还开源了大量实际使用的技能示例。对于希望构建自定义 AI 技能的开发者来说，这是不可多得的参考资源。

### 5.3 值得关注的点

1. **标准化格式**: SKILL.md 格式可能成为行业标准
2. **多平台支持**: 一次编写，处处运行
3. **企业级应用**: 文档处理技能已在生产环境使用

---

## 6. 资源与链接

### 6.1 官方资源

| 资源类型 | 链接 |
|---------|-----|
| GitHub | https://github.com/anthropics/skills |
| 文档 | https://support.claude.com/en/articles/12512176-what-are-skills |
| 创建技能指南 | https://support.claude.com/en/articles/12512198-creating-custom-skills |
| Agent Skills 标准 | https://agentskills.io |

---

## 7. 附录

### 7.1 更新日志

| 日期 | 更新内容 |
|------|---------|
| 2026-03-04 | 首次创建 |
