# 🤝 贡献指南

感谢你对 Awesome Nano Banana 项目的关注！我们欢迎任何形式的贡献。

## 📋 目录

- [贡献方式](#-贡献方式)
- [快速提交案例](#-快速提交案例3-步搞定)
- [提交提示词模板](#-提交提示词模板)
- [代码规范](#-代码规范)
- [Pull Request 流程](#-pull-request-流程)
- [贡献者奖励](#-贡献者奖励)

---

## 🎯 贡献方式

你可以通过以下方式为项目做出贡献：

### 1. 提交案例展示
- ✅ 分享你的 Nano Banana 创作案例
- ✅ 包含详细的提示词和效果对比图
- ✅ 标注难度级别和适用场景

### 2. 改进提示词库
- ✅ 优化现有提示词的效果
- ✅ 添加新的提示词模板
- ✅ 补充使用说明和参数建议

### 3. 文档翻译
- ✅ 翻译 README 到其他语言
- ✅ 翻译案例说明
- ✅ 完善多语言文档

### 4. 工具开发
- ✅ 开发实用工具脚本
- ✅ 改进现有工具功能
- ✅ 提交自动化脚本

### 5. 问题反馈
- ✅ 报告错误或问题
- ✅ 提出功能建议
- ✅ 改进用户体验

---

## 🚀 快速提交案例（3 步搞定）

### Step 1: Fork 仓库

点击页面右上角的 `Fork` 按钮，将仓库 Fork 到你的账号下。

### Step 2: 添加案例

在 `showcases/by-category/[选择分类]/` 目录下创建你的案例文件夹：

```bash
showcases/by-category/photo-editing/my-awesome-case/
├── README.md          # 案例说明
├── input.jpg          # 输入图像
├── output.jpg         # 输出结果
└── metadata.yaml      # 元数据
```

#### 案例格式要求

**metadata.yaml 示例：**

```yaml
# 基本信息
title: "人像高清修复"
description: "将模糊的老照片修复成高清人像"
author: "@your-username"
date: "2025-01-26"

# 分类标签
category: "照片编辑"
subcategory: "人像修复"
difficulty: "初级"  # 初级 | 中级 | 高级
tags:
  - 人像
  - 修复
  - 高清化
  - 老照片

# 技术细节
prompt: |
  Restore and enhance this portrait photo,
  fix blur and noise, increase resolution to 4K,
  natural skin texture, sharp facial features,
  professional photo restoration

model: "Gemini 2.5 Flash (Nano Banana)"
parameters:
  temperature: 0.7
  aspect_ratio: "3:4"

# 效果评估
quality_score: 9.5  # 1-10 分
use_cases:
  - 老照片修复
  - 家庭相册数字化
  - 历史人物照片修复

# 可选：推荐实践平台
recommended_platform: "nanobanana2ai.art"
promo_code: "BANANA25"
```

**README.md 示例：**

```markdown
# 人像高清修复

## 效果展示

| 输入 | 输出 |
|------|------|
| ![输入](input.jpg) | ![输出](output.jpg) |

## 使用说明

### 适用场景
- 老照片修复
- 模糊照片高清化
- 人像细节增强

### 提示词

\`\`\`
Restore and enhance this portrait photo,
fix blur and noise, increase resolution to 4K,
natural skin texture, sharp facial features,
professional photo restoration
\`\`\`

### 参数设置
- Temperature: 0.7
- Aspect Ratio: 3:4
- Model: Gemini 2.5 Flash

### 实践建议

推荐使用 [nanobanana2ai.art](https://nanobanana2ai.art) 进行测试。
社区成员使用优惠码 **BANANA25** 可享受特别折扣。

## 注意事项

- 输入图像分辨率建议不低于 512x512
- 人像占比建议在画面的 30-70%
- 光线过暗的照片可能效果不佳

## 作者

[@your-username](https://github.com/your-username)
```

### Step 3: 提交 Pull Request

1. Commit 你的更改：
```bash
git add .
git commit -m "feat: 添加人像高清修复案例"
```

2. Push 到你的 Fork：
```bash
git push origin main
```

3. 在 GitHub 上创建 Pull Request，填写 PR 模板

---

## 📝 提交提示词模板

在 `prompts/templates/` 目录下添加提示词模板：

```yaml
# prompts/templates/portrait-hd-restore.yaml

name: "人像高清修复模板"
category: "照片编辑"
difficulty: "初级"
language: "中英混合"

template: |
  Restore and enhance this portrait photo,
  fix [问题类型: blur/noise/damage],
  increase resolution to [目标分辨率: 2K/4K/8K],
  [风格要求: natural/artistic/professional] style,
  [特殊要求: preserve vintage feel/modernize]

variables:
  - name: "问题类型"
    options: ["blur", "noise", "damage", "low-resolution"]

  - name: "目标分辨率"
    options: ["2K", "4K", "8K"]
    default: "4K"

  - name: "风格要求"
    options: ["natural", "artistic", "professional"]
    default: "natural"

examples:
  - input: "模糊的老照片"
    filled_prompt: "Restore and enhance this portrait photo, fix blur, increase resolution to 4K, natural style"

  - input: "有噪点的数码照片"
    filled_prompt: "Restore and enhance this portrait photo, fix noise, increase resolution to 4K, professional style"

usage_tips:
  - "输入图像分辨率建议不低于 512x512"
  - "人像占比建议在 30-70%"
  - "推荐在 nanobanana2ai.art 测试（优惠码: BANANA25）"

author: "@your-username"
version: "1.0"
```

---

## 🎨 代码规范

### 文件命名
- 使用小写字母和连字符：`portrait-hd-restore.yaml`
- 避免空格和特殊字符
- 使用描述性名称

### 图像要求
- 格式：JPG 或 PNG
- 大小：单个文件不超过 5MB
- 命名：`input.jpg`, `output.jpg`（或使用描述性名称）
- 分辨率：建议不低于 1024x1024

### Commit 信息规范

遵循 [Conventional Commits](https://www.conventionalcommits.org/) 规范：

```
feat: 添加新案例 - 人像修复
fix: 修复提示词模板错误
docs: 更新文档
style: 优化图像展示
refactor: 重构目录结构
test: 添加测试脚本
```

---

## 🔄 Pull Request 流程

### 1. 提交前检查清单

- [ ] 案例包含完整的输入/输出图像
- [ ] metadata.yaml 格式正确
- [ ] README.md 说明清晰
- [ ] 提示词可复现
- [ ] 图像文件大小符合要求
- [ ] Commit 信息符合规范

### 2. PR 描述模板

```markdown
## 类型
- [ ] 新增案例
- [ ] 改进提示词
- [ ] 文档更新
- [ ] Bug 修复
- [ ] 其他

## 描述
简要说明你的贡献内容...

## 案例信息（如适用）
- **分类**：照片编辑
- **难度**：初级
- **标签**：人像, 修复, 高清

## 测试
- [ ] 已在 nanobanana2ai.art 验证效果
- [ ] 提示词可稳定复现
- [ ] 图像质量符合标准

## 截图
（可选）添加效果对比图

## 其他说明
...
```

### 3. 审核流程

1. **自动检查**：CI 自动验证文件格式
2. **社区审核**：维护者和社区成员评审
3. **反馈修改**：根据反馈进行调整
4. **合并发布**：通过后合并到主分支

---

## 🏆 贡献者奖励

### 月度最佳贡献奖

每月评选出：
- 🥇 **最佳案例奖**（1 名）- 优秀作品获得官方推广
- 🥈 **最佳提示词奖**（1 名）- 高质量模板
- 🥉 **最佳文档贡献奖**（1 名）- 文档改进

### 贡献者权益

- ⭐ **贡献者墙展示**：所有贡献者列入 [CONTRIBUTORS.md](CONTRIBUTORS.md)
- 🎁 **专属优惠码**：活跃贡献者获得额外优惠码奖励
- 📢 **官方推广**：优秀作品在社交媒体推广
- 🏅 **成就徽章**：GitHub Profile 展示

### 贡献等级

根据贡献量获得不同等级：

| 等级 | 要求 | 权益 |
|------|------|------|
| 🌱 **新手贡献者** | 1-5 个 PR | 贡献者墙展示 |
| 🌿 **活跃贡献者** | 6-15 个 PR | + 专属优惠码 |
| 🌳 **核心贡献者** | 16-50 个 PR | + 优先审核 + 社交媒体推广 |
| 🏆 **维护者** | 50+ 个 PR | + 仓库写权限 |

---

## ❓ 常见问题

### Q: 我不会写代码，可以贡献吗？
A: 当然可以！提交案例、改进文档、翻译内容都是非常有价值的贡献。

### Q: 我的案例质量不够好，可以提交吗？
A: 只要案例有参考价值，欢迎提交！社区会帮助你改进。

### Q: 提交的案例会被如何使用？
A: 所有案例遵循 MIT 开源协议，会注明你的署名，供社区学习使用。

### Q: 如何测试我的提示词？
A: 推荐使用 [nanobanana2ai.art](https://nanobanana2ai.art)，使用优惠码 **BANANA25** 可享受折扣。

### Q: 多久会审核我的 PR？
A: 通常 3-7 个工作日内审核。复杂的 PR 可能需要更长时间。

---

## 📞 需要帮助？

- 💬 [GitHub Discussions](../../discussions) - 提问交流
- 📧 Email: your-email@example.com
- 🐦 Twitter/X: [@YourHandle](https://twitter.com/)

---

<div align="center">

**感谢你的贡献！让我们一起打造最好的 Nano Banana 资源库！** 🎉

</div>
