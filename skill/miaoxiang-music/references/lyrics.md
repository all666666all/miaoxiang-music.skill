# 歌词创作参考 (Lyrics)

先词后曲 is the dominant AI workflow: precise lyric structure + section notes steer the model directly. Read this when writing or refining lyrics, engineering a hook (金句), fixing rhyme, or using 诗词 句式.

## Table of contents
- Structured writing + sectional prompts
- Formatting rules
- Rhyme optimization (押韵)
- Meaning/imagery optimization (寓意)
- 金句/hook engineering (3 types + 4 universal formulas)
- 诗词 句式 (4/5/6/7/8-言 + 顿点)
- Collaborating with AI 作词 (妙响 + 豆包/Gemini)

---

## Structured writing + sectional prompts

Use English section names with the model: **Intro** (基调/氛围, usually no main lyrics), **Verse** (主体故事/情感, same melody pattern repeats), **Chorus** (最具辨识度, repeats, holds the **hook**), **Bridge** (后半段, 不同旋律/节奏, 增加深度), **Outro** (收尾, 渐弱), **Pre-Chorus** (主→副过渡, 建立张力), **Interlude** (无词器乐过渡).

Common order: 前奏→主歌→前副歌→副歌→间奏→主歌→副歌→桥段→副歌→尾奏. RAP and EDM orders differ (see genres.md).

**Sectional prompts:** above each section, add an English `[ ]` directive describing that section's 编曲/情绪/特效, reflecting the song's natural development — sparse intro, full chorus, contrasting bridge, resolving outro. Place the directive **directly above** the lyrics:
```
[Verse 1][soft piano intro, clean and intimate vocal delivery, sparse instrumentation]
圈圈圆圆圈圈
天天年年天天的我

[Chorus][driving pop-rock drum beat enters, signature string section swells, powerful layered lead vocals, building emotional intensity]
不懂爱恨情愁煎熬的我们
```

---

## Formatting rules

- Meta tags `[verse]`/`[chorus]` are case-insensitive.
- 4–8 lyric lines per section generates best (no hard rule).
- Blank line between sections.
- `()` for ad-libs / 旁白 / 即兴.
- ~5–7 chars per line is comfortable; if AI sings "挤", your line is too long.

---

## Rhyme optimization (押韵) — "韵律服务于情感，押韵不绊住表达"

**Pick the 韵部 by emotion (韵母 has an emotional color):**
- 开口呼 (a, ang, ao, an): 洪亮开阔 → 大气/激昂/抒情 (望/光/茫/乡).
- 闭口呼 (i, in, ing, ü): 细腻内敛 → 温柔/伤感/叙事 (你/里/息/忆).
- 短促韵 (e, o, uo): 轻快干脆 → 活泼/俏皮/说唱 (乐/窝/火/阔).
- Keep a song's core 韵部 to **1–2 (max 3)** to avoid breaking the rhythmic feel.

**Use rhyme flexibly:**
- 完美韵 (韵母全同: 光-望-茫) → 副歌尾句 / 标题句, strengthen the memory hook.
- 斜韵 (韵母相近: 梦-懂, 走-久, 河-火) → 主歌/过渡, reduce 刻意感, keep it conversational.
- Don't rhyme every line; in 主歌叙事, rhyming every 2 or 4 lines breathes better (疏密结合).

**Change rhyme by section/emotion:** 主歌 loose 隔句押 (口语化: 天/边/烟); 副歌 dense 句句押 (冲击完美韵: 伤/慌/忘); 桥段 brief new 韵 for a turn (an→i). 情绪递进: 内敛 i 韵 (忆/里/寂) → 开阔 ang 韵 (光/茫/放).

**Avoid the rhyme traps:** ① 拒绝颠倒语序 (don't break natural word order to rhyme); ② replace 生僻韵脚 with common chars (龠→月, 玥→约); ③ check 倒字 — match 声调 to melody (平声配平缓, 仄声配起伏); ④ **留白不押韵** on the most honest/intense line (真实感 > 韵律感).

**进阶: 韵脚即意象** — make the rhyme word itself carry an image. For 离别 use 帆/岸/叹 (related images) over 饭/慢/看 (unrelated). Example fix: `有点淡`→`发着颤` (微动作, 更不舍); `湿汗`→`褶皱痕` (票根攥久的痕迹).

---

## Meaning/imagery optimization (寓意) — "从表达情绪到构建意象"

Don't say "我很难过"; build a scene the listener feels.
- **隐喻系统:** pick one core metaphor and run it through the whole song (社会压力 → 都市丛林/数字牢笼; 流水线=重复人生; 齿轮/螺丝钉=个体异化).
- **细节叙事+矛盾陈列:** replace slogans with concrete contradictory detail. ("为梦想付出很多" → "卖掉了收藏的球鞋换麦克风，在早餐钱和录音费间做选择困难症，妈妈的叹息是每晚的背景音").
- **语言陌生化:** 动词陌生化 ("时间在墙角霉变"); 名词动用 ("会议着整个人生"); 形容词化抽象 ("一段很水泥的沉默").
- **结构+留白:** Verse1 呈现 → Pre-Chorus 攀升 → Chorus 爆发(浓缩意象) → Verse2 深化/转折 → Bridge 升华/质疑 → Outro 余韵(意象收尾, 不说透). At peak emotion, *restrain* — a plain closing line hits harder.

**Two requirements of a strong lyric:** 逻辑感 + 画面感; focus emotion onto an individual so listeners self-insert. (镜头语言: 远景描写环境 + 近景聚焦个人情感 = 起承转合.) When AI writes generic/illogical phrases (便利店, 引擎低语, 体温线条), tell it to replace those specific words while keeping the rhyme.

---

## 金句/hook engineering — the single biggest virality lever

A 爆款 hinges on a 歌词金句 with three traits: **普适性** (covers everyone's emotion), **具象化** (scene/action/object, not abstract feeling words), **传播性** (works as a standalone caption/口播/签名). Core rule: **核心梗/hook out within ~15s, repeated 3+ times.**

**Three 金句 types:**
1. **热点锚定型** — borrow current-event traffic. Find hot points (抖音/快手热榜 8am/6pm, 抖音挑战榜 for 热梗, 微博 for 发酵源头, B站/百度/头条/音乐榜). Keep the original 梗 100% verbatim in the catchiest spot; extend it to a universal emotion so it breaks out of the meme circle. Formula: `热点原生核心梗 + 节奏对仗/重复强化 + 普适情绪延伸`.
2. **原创共情型** — say what people "心里有、嘴里无". Longest-lived (no 热点 dependency).
3. **经典复用型** — reuse classic lines/IP.

**Four universal 金句 formulas (原创共情):**
- **自我和解式** (全民共情最强): 我不必/不用【别人的期待/标准】，我只要【自己的选择/真实的样子】. e.g. "我不必开成所有人都爱的花，我可以做风吹不散的沙" (a 韵).
- **遗憾留白式** (情歌破防): 我还在【保留的习惯/旧场景】，只是【少了你的痕迹/回不去了】. e.g. "我还习惯点双人餐，只是对面空了一半" (an 韵).
- **细节扎心式** (画面感最强): 【旧物件/老场景】，藏着【没说出口的情绪】. e.g. "半瓶没喝完的酒，藏着没说出口的挽留" (iu 韵).
- **温柔自愈式** (短视频 BGM 首选): 【自然意象 风/雨/云/光】+【情绪治愈/和解】. e.g. "风会吹走所有遗憾，我会慢慢和自己和解" (an 韵).

**Hook-to-song checklist (replicable):** ① keep the 梗 verbatim in the catchiest spot, repeat throughout; ② 主歌 use real shared scenes so outsiders 共情; ③ 情绪有递进 (主歌压抑→预副歌推→副歌炸金句); ④ the 金句 must stand alone as a caption so people reuse it.

---

## 诗词 句式 (why some lyrics feel "对味")

Many beloved 华语 lyrics use 四/五/七言 句式 + 顿点 (the natural in-line pause that maps text to beats). 字数 = syllable count (汉字 only); 顿点 = the rhythmic split.

- **四言 (2+2)** — short, forceful, slogan-like; great for 洗脑 副歌/桥段 排比. ("我在/仰望，月亮/之上").
- **五言 (2+3 / 3+2)** — light, springy; 前半起画面, 后半落动作/情感. ("春风/过巷口").
- **六言 (3+3)** — balanced.
- **七言 (4+3 / 3+4)** — bigger emotional swing; 前四铺画面, 后三是情绪重心. ("我在春光/里等你").
- **八言 (4+4)** — long breath; "铺陈画面+情绪收束" in one line; ideal for 抒情副歌. ("桃红又是/一年春天").

心法: fit the right 字数 through clever 顿点 into the beat — get 顿点 right and it sings well. Mix 长短句 for rhythm.

---

## Collaborating with AI 作词

- **妙响 灵感模式 (首页):** put lyrics + style prompt together. Best for plain, well-understood 金句 (e.g. classical lines) — the model may not get the *newest* internet 梗.
- **妙响 AI作词 (高级模式):** chat "以【金句】为灵感，创作一首歌词". It returns a prompt + full lyrics. Default = one Verse + one Chorus (副歌可能进得快); ask for structure (e.g. "主歌分主歌1/主歌2再进副歌"). Edit unsatisfying lines directly. Click 使用歌词生成歌曲. **Don't set a BPM** when using AI 作词 — it auto-matches the lyric length; forcing a BPM makes it sound rushed.
- **External AI:** 豆包 (专家/超能模式 + 联网) understands Chinese internet 梗 / 出处 best; Gemini is better for 情感语录/原创/经典IP 改写 (also ask it to write a 妙响 style prompt). For illogical AI phrasing, instruct: "保留原本的韵脚，将 xxx 改为符合人类日常表达的字眼".
