# 曲风参考 (Genres)

Per-genre 万能公式, BPM ranges, key dimensions, and templates with full **structured (sectional)** examples. Read this when choosing/fusing a genre or when the user wants a genre template.

## Table of contents
- Quick genre selector
- 民族国韵 / 国风 (incl. 禅意/ambient — the BGM base)
- 潮流电子 EDM
- 动感流行
- Rap / 嘻哈
- Genre-by-BPM cheat sheet
- 7 common-style prompt skeletons (R&B / 抒情 / 舞曲 / DJ / 摇滚 / 国风 / Rap)
- AMBIENT / 梦核 / 怪核 BGM recipe (assembled for the 纯音乐 path)

---

## Quick genre selector

| Want | Genre | Formula head |
|---|---|---|
| 中国传统乐器 + 流行/影视/电子 | 民族国韵 | `[细分曲风]+[民族乐器]+[西方乐器/节奏]+[情绪意境]+[人声]` |
| 精良电子、可纯音乐 | EDM | `[BPM]+[节奏风格]+[标志音色]+[人声](选填)+[情感]` |
| 短视频"土嗨神曲"、下沉、强传播 | 动感流行 | `[BPM]+[节奏风格]+[标志音色]+[人声]+[情感]` |
| 说唱、与电子/国风可融合 | Rap/嘻哈 | `核心曲风+乐器编配+音色唱法+制作节奏+客观性` |
| 氛围/BGM/梦核/禅意 (纯音乐) | 国风禅意 + EDM ambient 词汇 | see last section |

动感流行 ≠ EDM: 动感流行 is a market concept (下沉受众, 情感直白, 极强传播); EDM is a genre (制作精良, 重音色设计, 可纯音乐).

---

## 民族国韵 / 国风

国风 isn't strictly a genre — it's a *method*: fuse Chinese traditional instruments with Pop/Rock/EDM/orchestral. 五声音阶 melody; lyrics 半文半白; 押韵/对仗.

**Formula:** `[细分曲风] + [核心民族乐器] + [西方现代乐器/节奏] + [情绪与意境] + [人声特征]`

**Key dimensions:**
- 配器: 拉弦 二胡/马头琴(+小提琴); 弹拨 古筝/琵琶/古琴(+吉他/竖琴); 吹管 笛子/洞箫; 打击 大鼓/木鱼/梆子.
- 调式: add `五声音阶 (Pentatonic)`, `东方旋律`, `中国民乐影响` to pull a Western-sounding melody back to "中国味".
- 意境: 空灵/禅意 (Ethereal, Zen, Atmospheric, Spiritual); 侠气/豪迈 (Wuxia, Heroic, Grand, Epic); 忧郁/思念 (Melancholic, Sentimental, Nostalgic); 唯美/清新 (Elegant, Graceful, Dreamy).
- BPM: 极速高燃 140–180+; 灵动洒脱 110–130; 标准叙事 85–105; 婉约感伤 65–80; **禅意意境 45–60 (禅意/仙侠空灵/纯古琴洞箫/BGM)**.
- Prefer Chinese prompts for 国风.

**Templates:**
- A 唯美抒情 (周杰伦/许嵩式): 华语流行, 中国风, 女声, 古筝与钢琴, 柔和弦乐, 五声音阶, 唯美忧郁, 钢琴铺底, 古筝/二胡勾勒旋律, 流行鼓点.
- B 宏大侠气: 史诗武侠原声, 宏大管弦乐, 笛子, 琵琶, 强力大鼓, 高能量, 英雄主义, 电影感.
- C 禅意空灵 (纯音乐): 纯音乐, 禅意, 古琴独奏, 洞箫, 极简主义, 空灵, 深层混响, 和平缓慢.
- D 新国风: 国风陷阱, 电子, 侵略性琵琶拨奏, 重低音808, 嘻哈节奏, 东方合成器, 融合风格.

**Structured example — 禅意山居 (Zen/Ambient Gufeng), 60 BPM** (the closest official model for ambient/梦核 BGM; vocals are a *texture*, not a lead):
```
[Intro]
[Music: A resonant Zen bell rings, echoing. Mountain birds and wind through bamboo. A deep, steady Guqin note begins.]

[Verse 1]
[Music: Solo Guqin, slow steady plucking. Heavy emphasis on silence between notes. Distant Xiao gives an occasional haunting accent.]
[Vocal: soft ethereal humming, no lyrics, following the pentatonic scale.]

[Pre-Chorus / Transition]
[Music: A subtle atmospheric pad slowly rises, infinite space. A soft wooden fish (Muyu) gives a steady meditative pulse.]
[Vocal: whispered, almost unintelligible, echoing.]

[Chorus / Peak]
[Music: Xiao takes a soaring melody. Guqin plays complex arpeggios. Light wind chimes shimmer in stereo.]
[Vocal: ethereal high vocalizing (Ahh/Ooh), smooth.]

[Outro]
[Music: Instruments peel away. Only mountain wind and a final soft Guqin remain.]
[End: total silence.]
```
Also available as structured examples in the source: 豪迈武侠 (140 BPM, Pipa+大鼓), 唯美抒情 (72 BPM, Erhu+soft piano), 新国风电子 (160 BPM, glitch Pipa + 808). Build them by the same pattern: `[section][Music: ...][Vocal: ...]`.

**国风 lyric craft:** 词库 by 意象 — 自然 (烟雨/残照/孤舟/长亭/落花/流年/江水/浮云); 器物 (纸伞/宣纸/朱砂/青衫/残剑/古琴/浊酒/锦书); 情感动词 (执剑/饮尽/勾勒/漂泊/轮回/相思/诀别); 地标色彩 (长安/江南/塞外; 黛色/朱红/墨韵/青花). Rhythm 4-2-4 or 5-7-5; ~5–7 chars/line; 多叠词 (悠悠/滚滚/冷冷清清). 半文半白 — neither pure 白话 nor pure 文言.

---

## 潮流电子 EDM

**Formula:** `[速度BPM] + [核心节奏风格] + [标志性音色] + [人声质感](选填) + [情感基调]`

- **细分:** House (Deep/Progressive), Techno (Acid/Peak Time), Future Bass (sawtooth 切分), Trance (史诗空间感).
- **BPM:** House 124–128; Techno 128–135; Future Bass 140–160; Drum&Bass 170–175.
- **音色设计:** Bass — Deep Sub Bass, Wobble Bass, Acid Synth. Synth — Pluck, Supersaw (慎用,高频刺耳), Arpeggio. Drums — Punchy Kick, 808, Crisp Snare.
- **氛围:** Euphoric, Melancholic, Aggressive, Cinematic, High Energy.
- **人声:** Pitched-up, Robotic, Ethereal female, Vocal chops.
- **混音母带:** Clean Mix, Wide Stereo, Punchy.
- Front-load `Aggressive, Heavy Drop` if you want it to bang. Use English for industry terms (Midtempo/Deep House).

**Templates:**
- A Future Bass/Melodic Dubstep: 未来低音, 150拍, 愉悦高燃, 华丽锯齿波, 强力808, 清脆打击乐, 旋律性起拍, 重低音Drop, 空灵女声切片, 专业母带.
- B Deep House/Chillstep: 深层浩室, 124拍, 深夜氛围, 忧郁且有律动, 温暖模拟低音, 丝滑钢琴音, 极简鼓点, 氛围铺底, 深情男声, 高级感.
- C Midtempo/Industrial 暗黑赛博: 中速低音电音, 100拍, 黑暗赛博, 侵略性粗糙合成器, 重度失真低音, 工业打击乐, 故障效果, 压抑紧张氛围.

EDM structure tags: `[Intro]`(只有鼓/简单合成器) `[Verse]`(人声) `[Build-up]` `[Drop]`(灵魂) `[Bridge]` `[Outro]`. For 纯音乐 omit `[Verse]`/`[Chorus]`.

---

## 动感流行

"土嗨神曲" — built for 短视频 BGM: 五声音阶, 口语化, 副歌前置, 片段化, used for 生活记录/剧情/舞蹈.

**Formula:** `[速度BPM] + [核心节奏风格] + [标志性音色] + [人声质感] + [情感基调]`

- 速度: 越南鼓疯狂感 135–140; Bounce 夜店 125–128.
- 节奏: 强劲底鼓 (Heavy kick), 反拍贝斯 (off-beat bass), 匀速四拍 (Four on the floor).
- 风格: 越南鼓 (Vina house), 车载DJ, 下沉 (cheesy EDM); 慢摇 (Chinese bounce), 夜店 (Night club), 劲爆浩室 (Slap House); 苦情 (Sad Mandopop), 民谣流行 (Folk-Pop), 中式流行 (Chinese pop).
- 音色: 合成器小号 (Synth brass), 冲击力打击乐, 民乐/古筝/笛子, 锯齿波领奏.
- 人声: 沙哑男声 (Raspy/Husky), 烟嗓 (Smoky), 重混响/回声, 高频人声切片.
- Vibe: 苦情 (Melancholic, Heartbreak, Sad lyrics); 土嗨热烈 (High energy, Club dance, Addictive hook).
- Prefer Chinese prompts (accurate 咬字).

---

## Rap / 嘻哈

Core paradigm = the **five elements** + 客观性 (see prompt-engineering.md). Common BPM 80–120 (range 85–160). Can fuse 电子/国风.

Example prompt: `这是一首华语嘻哈rap歌曲，自信的女声华语流行说唱与流畅的男声流行说唱交织，在E小调的轻快基调中融合华语流行与boombap元素。整体驱动、律动、充满能量，突出的贝斯线、紧凑鼓点与干净节奏吉他、钢琴构成核心律动，营造叙事感，以135 BPM推进。`

Rap structure: Intro → Verse1 → Pre-Chorus → Chorus/Hook → Verse2 → Pre-Chorus → Chorus/Hook → Bridge → Chorus/Hook → Outro.

---

## Genre-by-BPM cheat sheet

| 曲风 | 常见 BPM |
|---|---|
| R&B | 60–120 |
| 流行抒情 | 60–85 |
| 流行舞曲 | 100–130 |
| DJ | 120–150 |
| 摇滚 | 60–150 |
| 国风 | 60–130 (禅意 45–60) |
| 嘻哈 Rap | 80–120 (range 85–160) |
| House/Techno/Future Bass/DnB | 124–128 / 128–135 / 140–160 / 170–175 |

---

## 7 common-style prompt skeletons (from the 宝藏提示词 set)

- **R&B (60–120):** 气息轻柔女中音, G小调忧郁, 氛围感华语R&B, 带混响的洁净电吉他, 简单电子鼓点+深邃合成贝斯, 氛围合成器+抒情钢琴, 慢速, 感伤 lo-fi 质感. (swap 调性/性别; 电吉他→木吉他; lo-fi→灵魂乐即兴/80s R&B)
- **流行抒情 (60–85):** 清亮男高音, C大调明亮, 激励华语抒情, 轻柔钢琴引入→驱动摇滚鼓点+扎实贝斯, 史诗合成弦乐, 过载电吉他独奏, 情绪主歌→副歌攀升, 85 BPM, 电影配乐能量. (情感→忧郁; 融合中国乐器; 电吉他独奏→民谣吉他分解和弦)
- **流行舞曲 (100–130):** 冷艳气声女低音, C小调暗黑合成流行, 新迪斯科+电子舞曲, 驱动琶音合成贝斯, 铿锵电子鼓机, 氛围音墙, 抓耳合成器主旋律, 复古80s, 125 BPM. (暗黑→欢快/明朗效果完全不同)
- **DJ (120–150):** 真挚清澈女中音, C小调, 华语DJ+韩流舞曲, 强劲四四拍+冲击合成贝斯, 闪烁合成铺底+旋律琶音, 128 BPM. (调快到 130–150)
- **摇滚 (60–150):** 硬摇滚, 失真电吉他+突出贝斯+强力鼓点, 小调中速, 男声强劲略沙哑(主歌旋律/副歌近呐喊), 强力和弦+主奏段落+吉他独奏, 主歌-副歌+桥段+尾声, 原始能量混音清晰. (变 BPM/调式可大幅改变曲风; 加 riff/中国乐器)
- **国风 (60–130):** 中国古风流行, 曲速适中, 忧郁而充满希望, 古筝分解和弦贯穿, 钢琴延音和弦支撑, 清澈女高音+轻微颤音, 空灵合成垫音, 克制打击乐(柔和延音镲/锣点缀), 主歌副歌交替, 器乐间奏, 自然音阶, 干净清晰平衡.
- **嘻哈 Rap (80–120):** see Rap section.

---

## AMBIENT / 梦核 / 怪核 BGM recipe (assembled for the 纯音乐 path)

The knowledge base has no dedicated 梦核 genre — build it by combining the **国风 禅意空灵** template with **EDM atmospheric** vocabulary. This is the recipe for the swipe-feed / 短视频 BGM 纯音乐 strategy.

**Core parameters:**
- `Instrumental` / `纯音乐` (no lead vocals; optional wordless humming as a *texture* layer only)
- Slow: **45–60 BPM**, `极简/Minimalist`, `留白`, **no strong drums** (at most a soft Muyu/heartbeat pulse)
- Pads: `atmospheric synth pads`, `infinite space / 空灵 Ethereal`, `deep reverb`
- Signature color (pick to taste): 八音盒 (music box) / 失谐钢琴 (detuned piano) / 古琴 / 洞箫 / 卡西欧-style cheap synth / 远处模糊的古筝或笛子
- Texture signature: `老式磁带底噪 (tape hiss)`, `轻微电流声`, `lo-fi`, `褪色旧录像带质感`
- Emotion = the load-bearing dial: **"温暖怀旧 + 一丝不安"** (childhood-memory warmth + faint unease). Tune the 暖:诡 ratio (e.g. 7:3 warm-leaning 梦核 vs 5:5 darker 怪核).
  - 梦核 (Dreamcore): brighter, 怀旧 familiarity, lower review risk.
  - 怪核 (Weirdcore): darker, 诡异/不安, narrower use, higher review risk.
- **Hard BGM requirements:** `可无缝循环 (loopable)` and `≥60s` (also clears 汽水's 60-second counting threshold).

**Skeleton prompt (Chinese, 中式梦核 base):**
```
纯音乐，无人声。中式梦核氛围。怀旧八音盒与失谐钢琴动机，底层铺老式磁带的环境底噪与轻微电流声。情绪是熟悉又不安的临界感——童年记忆般的温暖，叠加一丝说不清的诡异。缓慢，留白多，无强节奏鼓点。音色偏暖但带轻微失真，像褪色的旧录像带。可无缝循环。时长60秒以上。
```
Variant axes to A/B (change ONE per test): 更暗(怪核 drone/空旷混响) · 更暖(八音盒主旋律清晰+儿童嬉闹环境声) · 换核心音色(卡西欧塑料感) · 加中式具象元素(古筝/笛子远景单音).

**Structure:** use the 简约意境 arrangement — `[Intro]-[Verse1]-[Interlude]-[Verse2]-[Chorus]-[Interlude]-[Outro]`, or for a pure loop just `[Intro]-[Build-Up(subtle)]-[Outro]` with musical tags only.
