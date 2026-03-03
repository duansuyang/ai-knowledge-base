---
title: Multi-Agent TODO Resolver
date: 2026-03-03
time: 22:45
source: GitHub
url: https://github.com/zclllyybb/multi-agent-todo
paper_url: 
github_url: https://github.com/zclllyybb/multi-agent-todo
tags: [Agent, Multi-Agent, Code, Development]
---

# Multi-Agent TODO Resolver - 多智能体代码助手

## 1. 项目概述

### 1.1 项目名称
Multi-Agent TODO Resolver

### 1.2 一句话概述
基于opencode的持久化多智能体系统，自动发现、计划、实施和审查代码变更

### 1.3 详细描述
一个持久化的守护进程多智能体系统，利用opencode自动发现代码库中的TODO/FIXME注释，通过Planner→Coder→Reviewer管道自动实现代码修复。多个任务并行运行，每个任务在独立的git worktree中执行

### 1.4 所属领域
- [x] Agent/I、工作流)
AG (智能体- [ ] LLM/大模型
- [ ] 多模态
- [ ] 强化学习
- [ ] 具身智能
- [ ] RAG/知识库
- [ ] AI安全
- [ ] 训练/部署
- [ ] 其他

### 1.5 标签
`#Agent` `#MultiAgent` `#CodeGeneration` `#OpenCode`

---

## 2. 项目来源

### 2.1 来源平台
- [x] GitHub
- [ ] arXiv 论文
- [ ] Hugging Face
- [ ] Papers with Code

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| 官方网站 | https://github.com/zclllyybb/multi-agent-todo |

### 2.3 发布时间
- 发布日期: 2026-03-02/03
- 发现日期: 2026-03-03

---

## 3. 项目优势

### 3.1 核心创新点

#### 创新点 1: 自动TODO发现与优先级排序
- **描述**: 扫描代码库中的TODO/FIXME注释，AI分析可行性评分，生成优先级待办列表
- **为什么重要**: 自动化代码维护工作流程

#### 创新点 2: Plan→Code→Review循环
- **描述**: 每个任务经过规划器(生成实现计划)、编码器(在隔离worktree中写代码)、审查者(批准或请求修改)的多轮迭代
- **为什么重要**: 确保代码质量，多重验证

#### 创新点 3: 多模型、多审查者
- **描述**: 根据任务复杂度分配不同模型(如Opus处理困难任务，Haiku处理简单任务)，多个审查者模型投票
- **为什么重要**: 成本效益与质量平衡

#### 创新点 4: 并行执行
- **描述**: 任务在独立git worktree分支中并发运行
- **为什么重要**: 提高效率，互不干扰

### 3.2 技术优势

| 优势类别 | 具体优势 | 量化指标 |
|---------|---------|---------|
| 自动化 | 自动TODO发现 | 支持 |
| 质量保证 | 多重审查机制 | 多模型投票 |
| 隔离性 | git worktree隔离 | 并行安全 |
| 交互性 | 人机协作 | 支持反馈重入 |

### 3.3 应用场景

1. **代码维护自动化**: 自动修复TODO/FIXME
2. **PR审查**: AI驱动的代码审查
3. **技术债务管理**: 识别和优先级排序
4. **团队协作**: AI辅助代码评审

### 3.4 适用人群
- [x] 开发者
- [x] 研究人员
- [ ] 企业/产品经理
- [x] 学生/学习者

---

## 4. 技术细节

### 4.1 架构

```
                         ┌──────────────────────────────────┐
                         │          Web Dashboard           │
                         │  (FastAPI, single-file HTML/JS)  │
                         └──────────┬───────────────────────┘
                                    │ REST API
                                    ▼
                         ┌─────────────────────┐
                         │     Orchestrator    │
                         └──────────┬──────────┘
```

### 4.2 核心组件

- **Web Dashboard**: 实时暗色主题UI，任务管理、agent运行检查、TODO浏览
- **Orchestrator**: 任务调度与协调
- **Planner**: 任务规划
- **Coder**: 代码生成 (在独立git worktree中)
- **Reviewer**: 代码审查

### 4.3 主要特性

1. 自动扫描TODO/FIXME并AI评分
2. Planner→Coder→Reviewer循环
3. 多模型配置
4. 并行任务执行
5. 人机协作
6. 运行时模型编辑
7. 资源生命周期管理

---

## 5. 总结与评价

### 5.1 项目评分

| 维度 | 评分 | 说明 |
|------|------|-----|
| 创新性 | ⭐⭐⭐⭐⭐ | 创新的多智能体代码维护方案 |
| 实用性 | ⭐⭐⭐⭐⭐ | 解决实际代码维护痛点 |
| 实验完整性 | ⭐⭐⭐ | 新项目，需更多验证 |
| 代码质量 | ⭐⭐⭐⭐ | 架构清晰 |

### 5.2 综合评价

Multi-Agent TODO Resolver是一个创新的多智能体代码维护系统。它通过自动发现代码库中的TODO注释，AI分析可行性，然后使用Planner→Coder→Reviewer管道自动实现修复。这种方案特别适合技术债务管理和日常代码维护场景。

### 5.3 值得关注的点

1. 自动化代码维护工作流
2. 多模型分配策略
3. Git worktree隔离保证安全
4. Web Dashboard可视化

### 5.4 下一步建议

- **如果你是开发者**: 在项目中尝试自动修复TODO
- **如果你是团队**: 集成到CI/CD流程

---

## 6. 附录

### 更新日志
| 日期 | 更新内容 |
|------|---------|
| 2026-03-03 | 首次创建 |
