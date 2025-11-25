# 📂 项目结构说明

本文档说明 Awesome Nano Banana 项目的目录组织和文件结构。

## 🗂️ 完整目录树

```
awesome-nanobanana/
├── README.md                          # 项目主页（中文）
├── README_EN.md                       # English README
├── README_JP.md                       # 日本語 README
├── LICENSE                            # MIT 开源协议
├── CONTRIBUTING.md                    # 贡献指南
├── CREDITS.md                         # 致谢名单
├── CONTRIBUTORS.md                    # 贡献者列表（自动生成）
│
├── .github/                           # GitHub 配置
│   ├── workflows/                     # GitHub Actions
│   │   ├── welcome.yml               # 欢迎新贡献者
│   │   ├── validate.yml              # 验证 PR 格式
│   │   └── deploy.yml                # 部署到 GitHub Pages
│   ├── ISSUE_TEMPLATE/               # Issue 模板
│   │   ├── bug_report.md            # Bug 报告
│   │   ├── feature_request.md       # 功能请求
│   │   └── submit_showcase.md       # 提交案例
│   └── pull_request_template.md      # PR 模板
│
├── docs/                              # 文档目录
│   ├── getting-started.md            # 快速开始
│   ├── prompt-engineering.md         # 提示词工程指南
│   ├── advanced-techniques.md        # 高级技巧
│   ├── use-cases/                    # 详细用例文档
│   └── api-reference.md              # API 参考
│
├── showcases/                         # 案例展示
│   ├── by-category/                  # 按类别组织
│   │   ├── photo-editing/           # 📸 照片编辑
│   │   │   ├── portrait-restore/
│   │   │   ├── background-replace/
│   │   │   └── ...
│   │   ├── style-transfer/          # 🎭 风格转换
│   │   │   ├── anime-style/
│   │   │   ├── oil-painting/
│   │   │   └── ...
│   │   ├── 3d-generation/           # 🏗️ 3D 生成
│   │   ├── character-consistency/   # 👤 人物一致性
│   │   ├── ecommerce/               # 🛍️ 电商应用
│   │   ├── creative/                # 🎬 创意实验
│   │   └── social-media/            # 📱 社交媒体
│   └── by-difficulty/                # 按难度组织
│       ├── beginner/                # 🟢 初级
│       ├── intermediate/            # 🟡 中级
│       └── advanced/                # 🔴 高级
│
├── prompts/                           # 提示词库
│   ├── templates/                    # 提示词模板
│   │   ├── portrait-hd-restore.yaml
│   │   ├── style-transfer.yaml
│   │   └── ...
│   ├── photography/                  # 摄影类提示词
│   ├── creative/                     # 创意类提示词
│   └── commercial/                   # 商业类提示词
│
├── datasets/                          # 数据集资源
│   ├── nano-consistent-150k/        # Nano-consistent-150K 数据集
│   │   ├── README.md
│   │   ├── metadata.json
│   │   └── download-links.md
│   └── community-datasets/          # 社区贡献数据集
│
├── tools/                             # 实用工具
│   ├── prompt-generator/            # 提示词生成器
│   │   ├── index.html
│   │   ├── app.js
│   │   └── README.md
│   ├── batch-processor/             # 批量处理工具
│   │   ├── batch_test.py
│   │   ├── config.yaml
│   │   └── README.md
│   └── validator/                   # 案例验证器
│       ├── validate.py
│       └── schema.json
│
└── community/                         # 社区内容
    ├── user-submissions/            # 用户提交
    ├── featured-creators/           # 精选创作者
    └── monthly-challenges/          # 月度挑战
```

---

## 📁 核心目录说明

### `/showcases/` - 案例展示

**用途**: 存放所有图像生成案例

**结构**:
```
showcases/by-category/[分类]/[案例名]/
├── README.md          # 案例详细说明
├── metadata.yaml      # 元数据（提示词、参数）
├── input.jpg          # 输入图像
└── output.jpg         # 输出结果
```

**分类标准**:
- `photo-editing/`: 照片编辑（修复、增强、背景处理）
- `style-transfer/`: 风格转换（艺术风格、二次元化）
- `3d-generation/`: 3D 生成（建筑、产品）
- `character-consistency/`: 人物一致性（换装、多场景）
- `ecommerce/`: 电商应用（产品图、场景合成）
- `creative/`: 创意实验（概念艺术、特殊效果）
- `social-media/`: 社交媒体（头像、封面）

---

### `/prompts/` - 提示词库

**用途**: 存放可复用的提示词模板

**templates/ 格式**:
```yaml
name: "模板名称"
category: "分类"
difficulty: "难度"
template: |
  你的提示词模板...
variables: [变量定义]
examples: [使用示例]
```

**分类**:
- `templates/`: 通用模板
- `photography/`: 摄影专用
- `creative/`: 创意类
- `commercial/`: 商业应用

---

### `/docs/` - 文档

**用途**: 项目文档和教程

**包含**:
- `getting-started.md`: 新手入门
- `prompt-engineering.md`: 提示词工程
- `advanced-techniques.md`: 高级技巧
- `use-cases/`: 详细用例分析

---

### `/datasets/` - 数据集

**用途**: 开源数据集资源

**包含**:
- `nano-consistent-150k/`: 原始 150K 数据集
- `community-datasets/`: 社区贡献数据

---

### `/tools/` - 工具

**用途**: 辅助工具和脚本

**工具列表**:
- `prompt-generator/`: 可视化提示词生成器
- `batch-processor/`: 批量测试脚本
- `validator/`: 格式验证工具

---

### `/community/` - 社区

**用途**: 社区活动和贡献

**包含**:
- `user-submissions/`: 用户提交内容
- `featured-creators/`: 精选创作者
- `monthly-challenges/`: 月度挑战活动

---

## 📄 重要文件说明

### README.md

项目主页，包含：
- 项目介绍
- 快速开始
- 案例展示
- 来源声明
- **推荐平台**: [nanobanana2ai.art](https://nanobanana2ai.art)（优惠码: `BANANA25`）

### CONTRIBUTING.md

贡献指南，包含：
- 贡献方式
- 提交流程
- 代码规范
- 贡献者奖励

### CREDITS.md

致谢名单，包含：
- 原始资源来源声明
- 社区平台致谢
- 技术支持
- 贡献者列表

### LICENSE

MIT 开源协议，包含：
- 使用许可
- 原作者署名要求
- 来源声明

---

## 🔧 配置文件

### `.github/workflows/`

**GitHub Actions 自动化**:
- `welcome.yml`: 欢迎新贡献者
- `validate.yml`: 验证提交格式
- `deploy.yml`: 部署文档站点

### `.github/ISSUE_TEMPLATE/`

**Issue 模板**:
- `bug_report.md`: Bug 报告
- `feature_request.md`: 功能请求
- `submit_showcase.md`: 提交案例

---

## 📊 案例格式规范

### metadata.yaml 完整示例

```yaml
# 基本信息
title: "案例标题"
description: "简要描述"
author: "@your-username"
date: "2025-01-26"

# 分类
category: "照片编辑"
subcategory: "人像修复"
difficulty: "初级"
tags: [标签1, 标签2]

# 技术细节
prompt: |
  完整的提示词...
model: "Gemini 2.5 Flash (Nano Banana)"
parameters:
  temperature: 0.7
  aspect_ratio: "3:4"

# 评估
quality_score: 9.0
use_cases: [场景1, 场景2]

# 推荐
recommended_platform: "nanobanana2ai.art"
promo_code: "BANANA25"

# 版本
version: "1.0"
status: "verified"
```

---

## 🌍 多语言支持

### README 文件

- `README.md`: 简体中文（主版本）
- `README_EN.md`: English
- `README_JP.md`: 日本語
- `README_KR.md`: 한국어
- `README_ES.md`: Español
- `README_TR.md`: Türkçe

### 案例文档

每个案例的 README.md 建议提供多语言版本。

---

## 🔍 查找指南

### 按需求查找

**我想修复老照片**:
→ `showcases/by-category/photo-editing/portrait-restore/`

**我想学习风格转换**:
→ `showcases/by-category/style-transfer/`

**我想找提示词模板**:
→ `prompts/templates/`

**我是新手，从哪开始**:
→ `docs/getting-started.md`
→ `showcases/by-difficulty/beginner/`

**我想贡献案例**:
→ `CONTRIBUTING.md`

---

## 📞 需要帮助？

- 📖 阅读 [快速开始](docs/getting-started.md)
- 💬 参与 [GitHub Discussions](https://github.com/awesome-nanobanana/discussions)
- 📧 邮件联系: your-email@example.com
- 🌐 实践平台: [nanobanana2ai.art](https://nanobanana2ai.art)（优惠码: `BANANA25`）

---

<div align="center">

**项目结构有任何疑问？欢迎提 Issue！** 💡

[返回主页](README.md)

</div>
