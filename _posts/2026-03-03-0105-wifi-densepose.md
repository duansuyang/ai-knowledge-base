---
title: wifi-densepose
date: 2026-03-03
time: 01:05
source: GitHub
url: https://github.com/ruvnet/wifi-densepose
tags: ["MultiModal", "Sensing", "Privacy", "Rust", "AI"]
---

# WiFi DensePose - 使用 WiFi 信号进行人体姿态估计

## 项目概述

WiFi DensePose 将普通 WiFi 信号转化为实时人体姿态估计、生命体征监测和存在检测——无需任何视频像素。通过分析人体运动引起的信道状态信息 (CSI) 扰动，系统利用基于物理的信号处理和机器学习重建身体位置、呼吸率和心跳。

## 核心功能

### 传感能力
- **姿态估计**: CSI 子载波幅度/相位 → DensePose UV 映射，54K fps (Rust)
- **呼吸检测**: 带通 0.1-0.5 Hz → FFT 峰值 6-30 BPM
- **心率检测**: 带通 0.8-2.0 Hz → FFT 峰值 40-120 BPM
- **存在感知**: RSSI 方差 + 运动频段功率，<1ms 延迟
- **穿墙感知**: Fresnel 区几何 + 多径建模，最深 5m

### 智能特性
- **自学习**: 从原始 WiFi 数据自学习，无需标注训练集
- **AI 信号处理**: 注意力网络、图算法、智能压缩
- **跨环境泛化**: 对抗域自适应，模型跨房间/建筑/硬件迁移
- **多视角融合**: 注意力融合多视角，减少身体遮挡

## 技术栈

| 组件 | 技术 |
|------|------|
| 语言 | Rust 53%, Python 25.9%, JavaScript 9.5% |
| 性能 | 54,000 frames/sec 流水线 |
| 部署 | Docker (132 MB), REST API, WebSocket |
| 硬件 | ESP32-S3 (~$54) 或研究级 NIC |

## 应用场景

- 🏥 医疗健康监测
- 🏪 零售客流分析
- 🔥 灾难救援 (穿墙探测被困人员)
- 🤖 机器人空间感知
- 🏠 智能家居存在检测

## 为什么重要

1. **隐私保护**: 无需摄像头，避免 GDPR/HIPAA 视频/成像规定
2. **穿墙能力**: WiFi 可穿透墙壁、货架、碎片
3. **成本低廉**: $0-$8/区域 vs 摄像头 $200-$2000
4. **无需硬件**: 现有 WiFi 或 $8 ESP32 即可部署

## 项目评分

| 维度 | 评分 | 说明 |
|------|------|------|
| 创新性 | ⭐⭐⭐⭐⭐ | 开创性的 WiFi 传感技术 |
| 实用性 | ⭐⭐⭐⭐⭐ | 多场景落地应用 |
| 实验完整性 | ⭐⭐⭐⭐ | 有完整代码和文档 |
| 代码质量 | ⭐⭐⭐⭐⭐ | Rust 重写，1031+ 测试 |

## 链接

- GitHub: https://github.com/ruvnet/wifi-densepose
- Docker: `docker pull ruvnet/wifi-densepose:latest`
- 演示: http://localhost:3000
