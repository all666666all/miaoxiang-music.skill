---
name: miaoxiang-music
description: >-
  Create AI music on 妙响 (MUSE SONG) — 汽水音乐 / 抖音音乐创作实验室's AI music
  platform. Use this skill WHENEVER the user wants to write music-generation
  prompts (提示词/structured prompts), pick or fuse a 曲风/genre (国风/民族国韵,
  EDM/电子, 动感流行, Rap/嘻哈, 禅意/ambient/梦核/纯音乐 BGM), write or refine song
  lyrics (歌词/金句/押韵/诗词句式), choose a generation model (Sway, SeedMusic,
  Mureka, MiniMax, TemPolor, Sodance, 音潮), troubleshoot AI output (唱错字/咬字/乱发挥),
  or optimize a track for 汽水 cold-start traffic (冷启/起量/完播率/30s跳出率/被选用/BGM).
  Trigger even when the user only describes the *outcome* (e.g. "help me make a
  creepy ambient BGM", "write me a viral hook", "why won't my new song get plays")
  without naming 妙响. Also trigger for batch/工作流/搬砖 music-generation planning.
---

# 妙响 (MUSE SONG) AI Music Creation

妙响 is 汽水音乐's one-stop AI music creation+distribution platform (前身 = 抖音音乐创作实验室). It is an AI DAW: AI 作曲 / AI 作词 / AI 和声 / AI 虚拟歌手 / 多轨精编 / 音频美化, with one-click 发行 to 抖音 + 汽水音乐. This skill encodes the official creation methodology so you can help users produce high-quality, platform-fit music.

## How to use this skill

Most requests fall into one of five jobs. Read the matching reference file(s) **before** writing prompts or lyrics — the references hold the parameter vocabularies, formulas, and templates that make output good.

| User wants… | Read |
|---|---|
| A music-generation prompt (style box or structured/分段) | `references/prompt-engineering.md` |
| To pick/fuse a genre, or a genre template (incl. 禅意/ambient/梦核 BGM) | `references/genres.md` |
| Lyrics, hooks (金句), rhyme (押韵), or 诗词 句式 | `references/lyrics.md` |
| The track to get plays / be picked as BGM on 汽水 | `references/distribution.md` |
| Platform features, model choice, or to fix bad output | `references/platform.md` |

When a task spans several (e.g. "make a viral 国风 song"), read several. Don't guess vocabulary from memory — the genre/instrument/effect terms in the references are what the models actually respond to.

## The core idea: structured prompting beats vibes

Saying "来点欢快音乐" gives random output. Locking each element — and ideally each *section* — into a structured prompt removes randomness. Two control surfaces:

1. **Global style prompt** (风格框) — defines overall style. Input in any of the platform's style fields.
2. **Sectional prompts** (分段指令 in the 歌词框) — per-section arranging/emotion/effects, wrapped in `[ ]`, placed directly above that section's lyrics. This lets you script the song's *arc* (sparse intro → full chorus → stripped bridge).

## The master prompt formula

```
[结构] + [风格] + [氛围] + [乐器] + [人声] + [其他细节]
```

Build it in four passes (骨架 → 皮肤 → 衣服 → 点缀):
1. **骨架** — structure tags + genre: `[Intro][Verse][Chorus]`, `80s Synth-pop`
2. **皮肤** — mood/emotion: `nostalgic and dreamy, for a late-night drive`
3. **衣服** — instruments + vocals: `led by a synth bassline and electronic drums, breathy female vocals`
4. **点缀** — effects/detail: `lush reverb, subtle tape saturation`

**Five must-have elements of any good prompt** (from the official Rap/宝藏 guides): 核心曲风 · 标志性乐器编配 · 音色与演唱技巧 · 制作与节奏特点 · **客观性** (describe concrete musical features; never subjective praise like "a great sound").

**Length:** 30–60 words is usually optimal. Over-long, contradictory prompts confuse the model. Often *simpler prompts generate better*.

**Hard-code vs. leave-open:** write an element explicitly when it's required (`male rap vocals`); use a broad word when you want AI latitude (`keyboard melody` instead of `piano melody`; `percussion` instead of `drum kit`).

**Language:** for genres that originated/peaked in China (国风, 动感流行, 苦情, DJ), prefer **Chinese** prompts — Chinese 咬字 comes out more accurate. For globally-named electronic terms (Midtempo, Deep House, Future Bass) use the **English** term for accuracy. Word order matters: front-loaded words carry more weight — put the most important descriptor first.

## The seven controllable dimensions (quick reference)

Full vocabularies in `references/prompt-engineering.md`. The seven: **1 乐器** · **2 人声** · **3 动态强度** · **4 氛围** · **5 环境音效** · **6 制作特效** · **7 其他参数 (BPM/拍号/调性/参考风格)**. For a pure-instrumental track, write `Instrumental` / `纯音乐` and omit the vocal block (or use it only for wordless 吟唱/humming as an atmosphere layer).

## Structure tags (use English `[ ]`; names must be correct)

`[Intro]` `[Verse]` `[Pre-Chorus]` `[Chorus]` `[Bridge]` `[Instrumental Break]/[Interlude]` `[Build-Up]` `[Drop]` `[Outro]`. Common arrangements:

- **经典抒情:** Intro-Verse1-PreChorus-Chorus-Verse2-PreChorus-Chorus-Bridge-Chorus-Outro
- **叙事长篇:** Intro-Verse1-Verse2-Chorus-Interlude-Verse3-Chorus-Chorus-Outro
- **史诗武侠:** Intro-Verse1-PreChorus-Chorus-InstrumentalBreak-Verse2-PreChorus-Chorus-Chorus-Outro
- **简约意境 (禅意/短视频纯音乐):** Intro-Verse1-Interlude-Verse2-Chorus-Interlude-Outro
- Viral tracks often **front-load the chorus** to grab the ear in the first seconds.

For a **纯音乐/instrumental**, drop `[Verse]`/`[Chorus]` lyric sections and use only musical tags (`[Intro]` `[Build-Up]` `[Drop]` `[Interlude]` `[Outro]`).

## Genre formulas (one line each — full versions in references/genres.md)

- **民族国韵/国风:** `[细分曲风] + [核心民族乐器] + [西方现代乐器/节奏] + [情绪与意境] + [人声特征]`
- **EDM/电子:** `[BPM] + [核心节奏风格] + [标志性音色] + [人声质感](选填) + [情感基调]`
- **动感流行:** `[BPM] + [核心节奏风格] + [标志性音色] + [人声质感] + [情感基调]`
- **Rap/嘻哈:** `核心曲风 + 标志性乐器编配 + 音色与演唱技巧 + 制作与节奏特点 + (客观性)`

**For ambient / 禅意 / 梦核 / 怪核 BGM** (the 纯音乐 path): start from the 国风 禅意空灵 template in `references/genres.md` and the EDM atmospheric/ambient vocabulary. Core recipe: slow (45–60 BPM), 极简/留白, no strong drums, atmospheric pads, optional 古琴/洞箫/八音盒 + magnetic-tape/lo-fi texture, "温暖怀旧 + 一丝不安" emotion. `可无缝循环 (loopable)` and `≥60s` are hard requirements for BGM.

## Lyrics, in one breath

先词后曲 is the dominant AI workflow. Key moves (full guide in `references/lyrics.md`): write **structured** lyrics (English section tags), add **sectional prompts** above each section, optimize **rhyme** (pick a 韵部 that matches the emotion; 1–2 韵部 per song; mix perfect + slant rhyme; leave the most honest line *unrhymed*), and build **imagery** not statements ("show, don't tell"). For virality, engineer a **金句/hook**: 普适性 + 具象化 + 传播性, repeated 3+ times, out in the first ~15s. 4/5/7-言 诗词 句式 (with 顿点) make hooks feel "对味". Lines of ~5–7 chars, 4–8 lines per section, blank line between sections, `()` for ad-libs/旁白. **Don't force a BPM when using AI 作词** — let it match the lyric length.

## Distribution reality (read references/distribution.md before advising on "起量")

汽水 is a swipe-to-listen feed; the algorithm pushes songs to users. Five metrics gate a new song: **30s 跳出率** (first-ear) · **完播率** · **互动率** (红心/评论/分享) · **收藏/使用率** (saved + used as BGM) · **转粉率**. For 搬砖/BGM creators the money lever is **使用率** (others picking your track as video BGM) → this is search-driven, so **song name + cover + scene tags** matter as much as audio. Name by *use-scene* ("中式梦核 童年回忆 BGM"), not by abstract/edgy titles (which also dodge content review). Get the hook out in the first 15–30s; don't bury it behind a long intro; trim dead 尾奏.

## Honest constraints to keep in view

- **客观性** in prompts, **show-don't-tell** in lyrics — these two principles drive most quality gains.
- Simpler often beats longer. If output is wrong, cut the prompt down before adding more.
- This skill describes the official creation method. It does **not** override platform rules or any signed agreement; never advise scripted/automated 刷量 (it is bannable). Real content driving real engagement is the only legitimate lever.
