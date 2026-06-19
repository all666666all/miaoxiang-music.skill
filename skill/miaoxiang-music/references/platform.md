# 平台参考 (Platform, Models, Fixes, Tools)

妙响's features, the generation-model lineup, troubleshooting recipes for bad AI output, and external helper tools. Read this for "how do I do X in 妙响", choosing a model, or fixing 唱错字/咬字/乱发挥.

## Table of contents
- Creation flow (NL + advanced)
- 制作优化 (vocal/track editing)
- 导出与发行
- 音乐改编 (翻唱/改词不改曲)
- Generation models (which to pick)
- Troubleshooting: 唱错字 / 咬字 / 乱发挥
- External tools

---

## Creation flow

妙响 = AI DAW. Two paradigms:

**Paradigm 1 — natural language (fastest):** 自然语言输入 → 灵感挑选 → 制作优化 → 作品发行.
1. 首页输入框: describe anything you want (≤500 chars); AI interprets.
2. 高级模式: enter a **style prompt** + **lyrics** separately (≤500 chars); or chat with the AI 作词 model to write lyrics.
3. 灵感挑选: each generation returns **2 results**; preview and 收藏 (五角星) the one you like.

**Paradigm 2 — structured/DAW:** for more control, use 分段提示词 in the 歌词框 and the multi-track editor (better suited to professional users).

---

## 制作优化 (vocal + track editing)

- **音轨分离:** right-click a track → 音轨分离 → 2轨 (人声 + 伴奏); separates editable vocal/instrumental stems.
- **智能演唱 (AI 虚拟歌手):** pick from **11 singers** (male/female 变声), or use 帮我推荐 — it suggests a singer based on your audio. The generated 智能演唱 is a **dry (干声)** vocal.
- **人声效果器:** 人声增强 / 特殊效果 / 音乐风格 — enhance & beautify vocals. Generated 智能演唱 has slight latency — nudge the audio earlier so the vocal 音头 aligns with the drum 音头.
- **智能和声:** map 人声 and 伴奏 tracks → top-tier 三度和声.
- **混响:** click a vocal clip → 轨道效果 → 混响; pick a type and drag 强度. Rough guide: 大厅混响 for 电子舞曲/金属; 房间混响 for R&B/民谣; 近距离混响 for 流行说唱.
- **变速变调:** 0.5×–1.5×.
- If output sounds "太干" / 音质不足: add 混响 in the AI 编辑器 and raise 增益 (loudness) to make the track stand out.

---

## 导出与发行

一键导出 + 直达抖音发行. After 创作, either 进 AI 编辑器 to edit then 发布 to 汽水, or 一键发布 directly to 汽水 from the 创作 module.

---

## 音乐改编 (翻唱 / 改词不改曲) — high value

When you love the generated 旋律+编曲 but need to fix something, use 音乐改编 instead of regenerating:
1. Click the song → 素材详情 → 快速改编 → 翻唱 (or 歌曲栏 编辑 → 翻唱).
2. The 歌词 panel auto-detects lyrics; fix the exact wrong chars precisely.
3. 风格描述: keep it short ("R&B", "流行") or empty — over-complex prompts backfire.
4. **高级选项:** to keep 人声旋律+伴奏 untouched and only change the wrong chars, set **参考音频权重 high (~8–9)** and 风格/创意发散 low. The 改编 also makes vocals more prominent/clearer (a quality bump). (前奏 配器 may shift slightly; to keep the original 前奏, cut+replace it in the AI 编辑器.)

---

## Generation models (which to pick)

Models differ by strength. Match the model to the job (especially vocal vs. instrumental, and language/style).

| Model | Strength | Best for |
|---|---|---|
| **Sway v5.5** | 音乐性+音质俱佳, 情绪细腻, **提示词遵循强**, 快速试听 | prompt-driven control; emotive tracks |
| **SeedMusic v4.3+** | 整体稳定, 人声优秀, **国风表现突出** | 国风/中式, batch consistency |
| **TemPolor v4.1a** | 音乐性+音质, 情绪细腻, **提示词遵循精确** | precise prompt control |
| **Sodance v2.0 preview** | 音乐性, 编曲层次, **为华语流行而生** (限时畅用) | 华语流行 |
| **Mureka v9** | 音质工艺, **华丽高超编曲, 贴合欧美流行** | lush/complex Western pop |
| **MiniMax v2.6** | **人声情绪丰富, 演唱细节强** | vocal-forward songs |
| **音潮 v3.0** | **音频续写/仿写**, 欧美/华语流行 | extending/imitating an existing track (great for 同质化系列化) |
| **TemPolor v4.0** | 多语种, 歌声灵动, 音质纯净 | multilingual vocals (superseded by 4.1a) |

Selection heuristics:
- **Prompt-following matters most** (you're steering via prompts) → Sway v5.5 / TemPolor v4.1a.
- **国风/中式/stability for batch** → SeedMusic v4.3+.
- **Pure instrumental / ambient** → models with strong 提示词遵循 + stability (Sway, SeedMusic, TemPolor); MiniMax is a poor fit (its edge is vocals). Mureka's "华丽编曲" fights ambient's 极简/留白.
- **Series/仿写 a found winner** → 音潮 v3.0 (续写/仿写).
- To compare models fairly: feed the **identical** prompt to each, generate **≥3** per model (single-shot mixes model差异 with run运气), score on fixed dimensions (e.g. for ambient BGM: 氛围契合 / 可循环性 / AI破绽 / 前3秒钩子). Use 快速试听 before committing full renders to save quota.

---

## Troubleshooting: 唱错字 / 咬字 / 乱发挥

When AI mis-sings a 多音字, slips into 粤语, or 吐字不清 ("落地窗"→"落的窗"):

1. **同音字替换** (if you accept regenerating melody/编曲): swap the troublesome char for a homophone ("稀"→"西"/"细"); tone差异 doesn't matter. Edit lyric only, keep the style prompt, regenerate → 风格大差不差.
2. **音乐改编 (推荐):** change-words-not-melody — see the 音乐改编 section above (参考音频权重 8–9). Best when you love the take.
3. **音色替换 (进阶, 网感/统一):** 音轨分离 (2轨) → 智能演唱, pick a target 音色 (or 帮我推荐) → add reverb to fit the 伴奏 → align 音头 to the beat. This swaps the vocal **timbre**; it does **not** fix wrong chars.

(For pure-instrumental tracks these vocal fixes rarely apply — regenerate or 改编 the 编曲 instead.)

---

## External tools

- **Gemini** (gemini.google.com): from a 歌手名 + 歌词, build a complete structured prompt for an AI music model; good for 情感语录/原创/经典IP 改写.
- **Sonoteller** (sonoteller.ai): paste a YouTube link or song+artist (English) → analysis report (主题/风格/氛围/配器/节奏) in 1–2 min. Use to reverse-engineer a reference track's prompt.
- **Every Noise at Once** (everynoise.com): 6000+ Spotify genres; click a word to hear an example, » jumps to that genre's artist map.
- **Chosic** (chosic.com): Spotify-library genre/search site (ad-heavy).
- **Music Map** (musicmap.info): genre timeline/lineage map for systematic style study.
- 豆包 (专家/超能 + 联网): best for understanding the newest Chinese internet 梗.
