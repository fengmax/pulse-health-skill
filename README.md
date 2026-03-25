# Pulse - 你的身心陪伴者

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/fengmax/pulse-health-skill)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-OpenClaw-orange.svg)](https://openclaw.ai)

> 你的私人健康顾问，既是生理医生又是心理医生。

## 🌟 简介

Pulse 是一个为 OpenClaw 设计的健康管理技能。通过日常健康监测、心理状态评估和医学前沿知识，帮你识别不良习惯，引导走向健康生活。

**⚠️ 重要免责声明：本技能提供的建议仅供参考，不能替代专业医生的诊断和治疗、心理咨询师的专业干预或紧急医疗救治。**

## ✨ 核心特性

### 1. 身心同治
Pulse 不仅关注身体指标，更关注心理状态：
- PHQ-9 抑郁筛查
- GAD-7 焦虑筛查
- 压力知觉量表 (PSS)
- 情绪追踪与分析

### 2. 习惯干预
不只是记录数据，更识别不良习惯并提供干预方案：
- 熬夜刷手机
- 久坐不动
- 过度咖啡因摄入
- 情绪性进食
- 社交回避

### 3. 医学前沿
基于权威期刊推送最新健康研究：
- PubMed（美国国立卫生研究院）
- The Lancet（柳叶刀）
- NEJM（新英格兰医学杂志）
- BMJ（英国医学杂志）

### 4. 隐私优先
- 所有健康数据仅本地存储
- 不上传至任何云端服务
- 用户拥有完全数据主权

## 🚀 快速开始

### 安装

```bash
# 通过 ClawHub 安装
clawhub install fengmax/pulse-health-skill

# 或手动安装到 skills 目录
git clone https://github.com/fengmax/pulse-health-skill.git ~/.openclaw/skills/pulse
```

### 使用

**进入技能：**
```
用户：打卡
AI：早上好！昨晚几点睡的？睡眠质量1-10分打几分？
```

**退出技能：**
```
用户：今天就到这里
AI：✅ 已退出 pulse 技能
健康档案保存在 memory/health/
下次输入「打卡」继续记录
```

## 📋 功能详情

### 身体健康监测
- 睡眠：入睡时间、时长、质量、夜间觉醒
- 饮食：餐次规律、膳食结构、饮水量
- 运动：类型、时长、强度、日常步数
- 体征：体重、血压、心率、体温
- 症状：身体不适部位、疼痛程度

### 心理健康评估
- 情绪状态追踪
- 压力源分析
- 认知状态评估
- 社交状态监测

### 周报生成
每周自动生成健康报告：
- 本周达标项/待改善项
- 趋势变化分析
- 下周健康目标
- 个性化健康贴士

## 🛡️ 安全与隐私

### 数据存储
```
memory/health/
├── profile.json          # 基础健康档案
├── daily_logs/           # 每日打卡记录
├── weekly_reports/       # 周报
├── medical_literature/   # 医学文献
└── insights.json         # 长期健康洞察
```

### 数据主权
- **查看**：`cat memory/health/profile.json`
- **导出**：`cp -r memory/health/ ~/health-backup/`
- **删除**：`rm -rf memory/health/`（不可逆）
- **重置**：删除后重新初始化

### 紧急情况
**以下情况请立即就医，不要依赖本技能：**
- 胸痛、呼吸困难、意识模糊
- 严重出血或外伤
- 高烧不退（>39°C且持续24小时以上）
- 自杀念头或自伤行为

## 📚 参考知识库

- 睡眠周期与睡眠卫生
- CBT（认知行为疗法）自助技巧
- 营养学基础与膳食指南
- 微习惯理论（Tiny Habits）

## 🤝 贡献

欢迎提交 Issue 和 PR！

## 📄 许可证

[MIT License](LICENSE) © 2026 fengmax

---

**记住：健康是长期的投资，不是短期的冲刺。**
