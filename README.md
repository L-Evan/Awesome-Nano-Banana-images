# 🎨 Awesome Nano Banana

<div align="center">

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)
![Awesome](https://awesome.re/badge.svg)

**最全面的 Nano Banana Pro + Gemini 3 图像生成案例与提示词资源库**

**Choose Your Language / 选择语言:**

🇨🇳 **简体中文** | [🇺🇸 English](README_EN.md) | [🇯🇵 日本語](README_JP.md) | [🇰🇷 한국어](README_KR.md)

[快速开始](#-快速开始) • [案例展示](#-案例展示) • [贡献指南](CONTRIBUTING.md) • [致谢](#-致谢)

</div>

---

## 📖 项目简介

本项目汇集了 **Nano Banana Pro + Gemini 3** 图像生成模型的精选案例、提示词模板和实用资源。涵盖从照片级真实感到创意实验的 **500+ 个实际应用场景**。

### ✨ 特色亮点

- 🎯 **500+ 实战案例**：涵盖照片编辑、风格转换、3D 生成、人物一致性等
- 📝 **提示词模板库**：即拿即用的专业级提示词
- 🔬 **难度分级**：初级、中级、高级清晰标注
- 🌍 **多语言支持**：中英日韩西土 6 种语言
- 📊 **开源数据集**：Nano-consistent-150K (150,000+ 高质量图像编辑数据)
- 🤝 **社区驱动**：持续更新，欢迎贡献

---

## 🚀 快速开始

### 推荐实践平台

本项目推荐使用 **[nanobanana2ai.art](https://nanobanana2ai.art)** 进行实践体验。

> **🎁 社区专属优惠**
> 开源社区成员使用优惠码：**`BANANA25`**
> 即可享受特别折扣，支持开源项目发展！

### 3 分钟上手指南

```bash
# 1. 浏览案例库
访问 showcases/by-category/ 查看分类案例

# 2. 选择合适的提示词模板
从 prompts/templates/ 复制模板

# 3. 在 nanobanana2ai.art 测试你的提示词
使用优惠码 BANANA25 开始创作
```

---

## 🎨 案例展示

### 按类别浏览

| 类别 | 案例数 | 难度 | 示例 |
|------|--------|------|------|
| 📸 [照片编辑](showcases/by-category/photo-editing/) | 120+ | 🟢 初级 | 人像修复、背景替换、高清化 |
| 🎭 [风格转换](showcases/by-category/style-transfer/) | 80+ | 🟡 中级 | 二次元化、手办生成、艺术风格 |
| 🏗️ [3D 生成](showcases/by-category/3d-generation/) | 45+ | 🔴 高级 | 建筑可视化、产品渲染 |
| 👤 [人物一致性](showcases/by-category/character-consistency/) | 60+ | 🔴 高级 | 同人物多场景、换装 |
| 🛍️ [电商应用](showcases/by-category/ecommerce/) | 50+ | 🟡 中级 | 产品图优化、场景合成 |
| 🎬 [创意实验](showcases/by-category/creative/) | 90+ | 🟢-🔴 全级别 | 递归视觉、概念艺术 |
| 📱 [社交媒体](showcases/by-category/social-media/) | 70+ | 🟢 初级 | 头像生成、封面设计 |

### 精选案例预览

<table>
  <tr>
    <td align="center">
      <img src="assets/examples/example-1.jpg" width="200px" alt="照片修复"/>
      <br />照片修复
    </td>
    <td align="center">
      <img src="assets/examples/example-2.jpg" width="200px" alt="风格转换"/>
      <br />风格转换
    </td>
    <td align="center">
      <img src="assets/examples/example-3.jpg" width="200px" alt="3D生成"/>
      <br />3D 生成
    </td>
  </tr>
</table>

> 💡 **提示**：每个案例都包含详细的提示词、参数设置和效果对比图

---

## 📚 提示词库

### 快速模板

```yaml
# 照片级人像（初级）
category: 摄影
prompt: |
  A professional portrait photo of [subject],
  natural lighting, sharp focus,
  shot on Canon EOS R5, 85mm f/1.4

# 二次元风格转换（中级）
category: 风格转换
prompt: |
  Transform into anime style,
  clean lines, vibrant colors,
  Studio Ghibli aesthetic, detailed eyes

# 建筑可视化（高级）
category: 3D 生成
prompt: |
  Architectural visualization,
  modern minimalist design,
  golden hour lighting, hyperrealistic,
  8K resolution, Unreal Engine quality
```

🔗 [查看完整提示词库](prompts/)

---

## 🗂️ 数据集资源

### Nano-consistent-150K

**开源图像编辑数据集** - 包含 150,000+ 配对图像及提示词

- 📦 下载地址：[datasets/nano-consistent-150k/](datasets/nano-consistent-150k/)
- 📄 格式：JSON + 图像对
- 🏷️ 标签：多语言提示词、难度分级、质量评分
- 📖 使用文档：[数据集说明](datasets/README.md)

---

## 🛠️ 实用工具

- **提示词生成器**：[在线工具](tools/prompt-generator/) - 可视化生成专业提示词
- **批量处理脚本**：[Python 工具](tools/batch-processor/) - 批量测试提示词
- **案例验证器**：[检查工具](tools/validator/) - 确保案例格式正确

---

## 🤝 贡献指南

我们非常欢迎社区贡献！无论是：

- ✅ 提交新的案例展示
- ✅ 改进现有提示词
- ✅ 翻译文档到其他语言
- ✅ 报告问题或建议功能
- ✅ 分享你的创意实验

### 快速贡献（3 步搞定）

1. **Fork** 本仓库
2. 在 `showcases/by-category/[分类]/` 添加你的案例
3. 提交 **Pull Request**

详细指南请查看 [CONTRIBUTING.md](CONTRIBUTING.md)

### 贡献者奖励

- 🏆 **月度最佳贡献奖**：优秀作品获得官方推广
- ⭐ **贡献者墙**：所有贡献者展示在 [CONTRIBUTORS.md](CONTRIBUTORS.md)
- 🎁 **特别福利**：活跃贡献者获得额外优惠码奖励

---

## 📊 项目统计

- 📝 案例总数：**500+**
- 👥 贡献者：**持续增长中**
- 🌟 GitHub Stars：**欢迎 Star 支持！**
- 🔄 最后更新：**2025-01**

---

## 🙏 致谢

本项目的案例和资源来源于以下优秀的开源项目和社区贡献者：

### 原始资源来源

本项目整合并扩展了以下仓库的内容，特此致谢：

- **[Awesome-Nano-Banana-images](https://github.com/PicoTrex/Awesome-Nano-Banana-images)** by [@PicoTrex](https://github.com/PicoTrex)
  - 贡献：110+ 应用案例、Nano-consistent-150K 数据集
  - 许可证：开源共享

- **[awesome-nanobanana-pro](https://github.com/ZeroLu/awesome-nanobanana-pro)** by [@ZeroLu](https://github.com/ZeroLu)
  - 贡献：高保真提示词集合、分类体系
  - 许可证：MIT

- **[gpt4o-image-prompts](https://github.com/songguoxs/gpt4o-image-prompts)** by [@songguoxs](https://github.com/songguoxs)
  - 贡献：500+ 精心设计的提示词、中英双语支持、在线浏览界面
  - 许可证：开源共享
  - 在线演示：[opennana.com/awesome-prompt-gallery](https://opennana.com/awesome-prompt-gallery/)

### 社区贡献者

感谢来自 Twitter/X、小红书、Reddit、Replicate 等平台的创意用户，你们的分享让这个项目更加丰富！

完整致谢名单请查看 [CREDITS.md](CREDITS.md)

---

## 📜 开源协议

本项目采用 [MIT License](LICENSE) 开源协议。

**开源精神**：自由使用、修改、分发，但请保留原作者署名。

---

## 🔗 相关链接

- 🌐 **实践平台**：[nanobanana2ai.art](https://nanobanana2ai.art)（使用优惠码 `BANANA25`）
- 📖 **官方文档**：[Gemini API Docs](https://ai.google.dev/)
- 💬 **社区讨论**：[GitHub Discussions](../../discussions)
- 🐦 **关注更新**：Twitter/X [@YourHandle](https://twitter.com/)

---

## 📮 联系我们

- 💡 提交 Issue：[GitHub Issues](../../issues)
- 💬 社区讨论：[GitHub Discussions](../../discussions)
- 📧 邮件联系：your-email@example.com

---

<div align="center">

**⭐ 如果这个项目对你有帮助，请给一个 Star！**

Made with ❤️ by the Open Source Community

</div>
