# 妙响 (MUSE SONG) AI 音乐 Skill

**中文| [English](README-ENG.md)**

---

一个 [Claude Skill](https://www.anthropic.com/news/skills)，封装了 **妙响 (MUSE SONG)**——**汽水音乐 / 抖音音乐创作实验室**旗下 AI 音乐创作发行平台——的音乐创作方法论。

安装后，Claude 可以帮你写音乐生成提示词、挑选与融合曲风、写歌词与金句、选择生成模型、排查 AI 输出问题，以及为汽水冷启起量做优化——无需每次都把参考资料粘贴进去。

---

## ⚠️ 来源与声明（请先阅读）

本项目是**非官方的社区学习辅助工具**。其内容**提炼并改写**自妙响 / 抖音音乐（字节跳动）官方面向创作者的知识库资料。它**不是**官方文档的逐字复制，也**与字节跳动、抖音、汽水音乐、妙响无任何隶属、背书或维护关系**。

- 所有商标（妙响、MUSE SONG、汽水音乐、抖音、Sway、SeedMusic 等）归各自所有者所有。
- 本仓库总结的方法论、公式与参数参考源自官方知识库，本仓库仅为方便学习而重新组织。
- 如你是权利方并希望下架或调整，请提交 issue。
- **时效性：** 基于截至 **2026-06** 的知识库资料。模型阵容、平台功能、流量规则变动频繁，可能已过时，请以官方最新文档为准。

请自行斟酌使用。本仓库内容不凌驾于平台服务条款或你签署的任何协议之上。

---

## 仓库内容

```
skill/miaoxiang-music/
├── SKILL.md                        # 总纲、任务路由、万能提示词公式、七大维度
└── references/
    ├── prompt-engineering.md       # 七维完整词库、组装方法、8 个模板
    ├── genres.md                   # 各曲风公式、BPM 区间、模板（含 ambient/梦核 BGM）
    ├── lyrics.md                   # 结构、押韵、意象、金句公式、诗词句式
    ├── distribution.md             # 汽水冷启：五大指标 + 调优招数、命名、账号运营
    └── platform.md                 # 功能、模型阵容、纠错、外部工具

dist/
└── miaoxiang-music.skill           # 打好的、可直接安装的成品包
```

## 安装

**方式 A —— 用打好的成品包（最简单）**
1. 下载 [`dist/miaoxiang-music.skill`](dist/miaoxiang-music.skill)。
2. 在 Claude（claude.ai 或桌面端）：**设置 → Capabilities/Skills → 上传** 这个 `.skill` 文件。（在 Claude Code 中，把解压后的 skill 文件夹放进你的 skills 目录。）

**方式 B —— 从源文件自行打包**
```bash
# 打包 skill 文件夹，使压缩包根目录即 skill 目录：
cd skill
zip -r ../miaoxiang-music.skill miaoxiang-music
```
然后按方式 A 上传生成的 `.skill`。

## 如何触发

你无需点名"妙响"。当你让 Claude 做以下事情时，skill 会自动激活：
- 写音乐生成提示词（提示词 / 结构化 / 分段）
- 挑选或融合曲风（国风/民族国韵、EDM/电子、动感流行、Rap/嘻哈、禅意/ambient/梦核 BGM）
- 写或润色歌词、金句、押韵、诗词句式
- 选择生成模型（Sway、SeedMusic、Mureka、MiniMax、TemPolor、Sodance、音潮）
- 排查 AI 输出问题（唱错字 / 咬字 / 乱发挥）
- 为汽水冷启做优化（冷启 / 起量 / 完播率 / 30s跳出率 / 被选用 / BGM）

……即使你只描述目标也会触发。

## 贡献

欢迎 issue 和 PR——尤其是平台模型、功能或规则变动后的勘误。请编辑 `skill/miaoxiang-music/` 下的**源文件**，而非打包好的 `.skill`。改动后用方式 B 的命令重新打包（并更新声明里的日期）。

## 许可

[MIT](LICENSE)，覆盖本仓库的**结构、措辞与组织方式**。该许可不授予任何第三方商标的权利，也不授予其所总结的官方底层资料的权利。
