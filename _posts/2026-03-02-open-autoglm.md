---
title: Open-AutoGLM - 开源手机智能体框架
date: 2026-03-02
time: 00:21
source: GitHub
url: https://github.com/zai-org/Open-AutoGLM
github_url: https://github.com/zai-org/Open-AutoGLM
tags: [Agent, Phone-Agent, Multimodal]
---

# Open-AutoGLM: 开源手机智能体

## 1. 项目概述

### 1.1 一句话概述
Open-AutoGLM 是智谱 AI 开源的手机智能体框架，能通过自然语言指令控制手机执行各种任务，如打开应用、搜索内容等。

### 1.2 详细描述
Phone Agent 基于 AutoGLM 构建，以多模态方式理解手机屏幕内容，通过 ADB 控制 Android 设备，结合视觉语言模型进行屏幕感知和智能规划。用户只需用自然语言描述需求，如"打开小红书搜索美食"，系统即可自动完成整个操作流程。

### 1.3 所属领域
- [x] Agent/IAG (智能体、工作流)
- [x] 多模态 (VLM、视觉理解)

---

## 2. 项目来源

### 2.1 来源平台
- [x] GitHub Trending

### 2.2 链接
| 链接类型 | URL |
|---------|-----|
| GitHub | https://github.com/zai-org/Open-AutoGLM |
| HuggingFace | https://huggingface.co/zai-org/AutoGLM-Phone-9B |
| 产品体验 | https://autoglm.zhipu.cn/autotyper/ |

### 2.3 关键数据
- **Stars**: 23,863
- **Forks**: 3,777
- **创建时间**: 2025-12-08

---

## 3. 核心创新

### 3.1 核心能力
| 能力 | 说明 |
|------|-----|
| 多模态屏幕理解 | VLM 理解手机界面 |
| 自然语言控制 | 用自然语言描述任务 |
| 自动操作规划 | 自动生成操作序列并执行 |
| 敏感操作确认 | 内置安全确认机制 |
| 人工接管 | 登录/验证码场景支持人工介入 |

### 3.2 技术架构
1. **屏幕感知**: 视觉语言模型理解当前界面
2. **意图解析**: 理解用户自然语言需求
3. **动作规划**: 生成操作步骤序列
4. **执行控制**: 通过 ADB/HDC 执行操作

### 3.3 支持设备
- Android 7.0+ (ADB)
- 鸿蒙 NEXT 以上版本 (HDC)

---

## 4. 模型下载

| 模型 | 说明 |
|------|-----|
| AutoGLM-Phone-9B | 中文手机应用优化版 |
| AutoGLM-Phone-9B-Multilingual | 多语言支持版 |

---

## 5. 应用场景

1. **日常手机操作**: 搜索、导航、订餐
2. **自动化测试**: UI 自动化测试
3. **无障碍辅助**: 语音控制手机
4. **企业流程自动化**: 批量处理手机任务

---

## 6. 总结

**创新性**: ⭐⭐⭐⭐⭐ 首个开源手机智能体方案
**实用性**: ⭐⭐⭐⭐⭐ 已产品化落地
**代码质量**: ⭐⭐⭐⭐ 文档完善

**适合人群**: 移动开发者、AI 爱好者、自动化工程师

**链接**: https://github.com/zai-org/Open-AutoGLM
