# 提示词工程参考 (Prompt Engineering)

Full vocabularies for the seven controllable dimensions, the assembly method, and worked templates. Read this whenever writing a global style prompt or sectional (分段) prompts.

## Table of contents
- The two control surfaces
- Five must-have elements + 客观性
- The seven dimensions (full vocab)
- Assembly method (4 passes)
- Hard-code vs. leave-open / length / language / word order
- Sectional-prompt format
- 8 copy-ready templates

---

## The two control surfaces

1. **全局风格提示词 (style box):** defines overall style. The platform exposes style input in three places; any works.
2. **分段提示词 (in the 歌词框):** per-section directives in `[ ]`, placed on the line **directly above** that section's lyrics. They must reflect the song's natural development: `[Intro]`/`[Verse 1]` sparse & simple (`soft piano intro, intimate vocal`); `[Chorus]` fuller & higher-energy (`full band enters, powerful layered vocals`); `[Bridge]` contrast (`instrumentation strips back, emotive falsetto`); `[Outro]` resolution.

You can put **arranging** and **vocal** directives in separate bracketed lines, e.g.
```
[Music: ...]
[Vocal: ...]
```

---

## Five must-have elements of a good prompt

1. **核心曲风 (Core Genre)** — R&B, 摇滚, 爵士, Trap, Deep House…
2. **标志性乐器编配 (Signature Instrumentation)** — 氛围合成器, 击弦贝斯, 钢琴, 弦乐群…
3. **音色与演唱技巧 (Vocal Timbre & Technique)** — 气声, 假音, 呐喊式, 呢喃式叙事腔, 情感颤音…
4. **制作与节奏特点 (Production & Rhythmic Feel)** — 电影感制作, 极简氛围, 滞后于节拍的律动…
5. **客观性 (Objectivity)** — describe concrete musical features only. Never write subjective praise/summary ("一种伟大的声音", "超好听"). This single rule prevents a lot of muddy output.

Knowing genre rules matters: mismatched elements (e.g. "硬核说唱嘶吼" inside "极简氛围 R&B") confuse the model. Keep 曲风/乐器/情绪 mutually coherent.

---

## The seven dimensions (full vocabulary)

### 1. 乐器 Instrumentation (the flesh)
- **节奏组 Rhythm:** Drums — Drum Kit, 808 Drums, Acoustic Drums, Electronic Drum Machine, Hand Percussion. Bass — Electric Bass, Synth Bass, Acoustic Bass (低音提琴), Funky Bassline.
- **和声/旋律 Harmony & Melody:** Guitar — Acoustic Guitar, Electric Guitar (+Clean/Distorted/Crunchy), Lead Guitar Solo. Keys — Piano, Electric Piano, Organ, Synthesizer (+Pads/Leads/Arpeggiator).
- **管弦 Orchestral:** String Section, Violin, Cello, Brass Section, Trumpet, Orchestral Hit.
- **世界/特色 World & Exotic:** Ukulele, Sitar, Shakuhachi (尺八), Guzheng (古筝), Kalimba.
- Write-up: mark priority with `led by` / `with` — `led by a gentle acoustic guitar, with a soft bass and light percussion`. Group related instruments — `distorted electric guitars, a powerful drum kit, and a heavy bassline`.

### 2. 人声 Vocals (the soul — describe precisely)
- **有无:** Vocal / Instrumental (纯器乐).
- **性别+音色:** Male / Female; Deep, Raspy, Breathy, Angelic, Clear, Powerful, Soothing.
- **和声/伴唱:** Harmonies, Backup Vocals, Ad-libs, Choir.
- **唱法:** Narrative, Rapping, Belting, Whispering, Melismatic (花腔), Falsetto.
- **语言:** English (default), Mandarin, Japanese, K-pop, Non-Lyrical Vocals (无意义吟唱), Oohs and Aahs.
- **主导性:** vocal-led → put singing descriptor first (`Rapping male vocals over a boom-bap beat`); vocal-as-texture → treat as instrument (`Dreamy synthwave with breathy female vocal pads`).

### 3. 动态强度 Dynamics
- 整体: Mellow, Energetic, Intense, Calm, Aggressive.
- 力度曲线: 渐强 (Gradual build-up, Slow burn, Layer by layer); 爆发 (Explosive chorus, Powerful drop, Epic crescendo); 渐弱 (Fade out, Decrescendo, Stripped back).
- 段落: `[Verse][calm and sparse]`, `[Chorus][explosive and dense]`, `[Bridge][quiet and reflective, then builds into the final chorus]`.

### 4. 氛围 Mood & Vibe (most creative)
- 情绪: Uplifting, Melancholic, Hopeful, Nostalgic, Anxious, Romantic, Playful.
- 场景/色彩: Epic, Dreamy, Futuristic, Retro, Vintage, Cinematic, Lo-fi, Urban night, Sunny morning, Sci-fi cold, Cyberpunk.
- Combine 场景+情绪 for unique vibes (`Nostalgic retro vibe`). Be concrete: `Music for a late-night drive in Tokyo` beats `Urban night`.

### 5. 环境音效 Sound Effects / Ambience (immersion)
- City street, Rain, Wind, Ocean waves, Crowd noise, Nature ambience, Mechanical rhythm, Vinyl crackle (黑胶炒豆声).
- Uses: subtle bg (`...with a subtle vinyl crackle in the background`); as intro/transition (`[Intro][starts with the sound of rain, then a sad piano enters]`); foreground swap (waves move to foreground in the bridge).

### 6. 制作特效 Production Effects (the seasoning)
- 空间: Reverb (Lush/Hall reverb), Delay.
- 失真/饱和: Distortion, Overdrive, Fuzz, Tape Saturation (复古暖意).
- 动态/节奏: Sidechain compression (EDM pump), Gated reverb (80s drums).
- 滤波/故障: Filter sweep, Low-pass filter (闷), Glitch effects, Stutter.
- 质感: Lo-fi, Bit-crushed.
- Genre combos: EDM — `heavy sidechain compression, big reverb, filter sweeps, delay on vocals`; Vintage Rock — `tape saturation, spring reverb, light overdrive on guitars`; Hip Hop — `lo-fi texture, vinyl crackle, deep 808 bass with distortion`.

### 7. 其他参数
- **速度 Tempo:** explicit `120 BPM`; or `slow (~60-80)`, `mid (~90-110)`, `up-tempo (>120)`; words: Relaxed, Driving, Hectic.
- **拍号 Meter:** 4/4 (default), 3/4 (waltz), 6/8 (slow rock).
- **调性 Key:** Major (sunny), Minor (melancholic), Modal.
- **参考风格 Style:** `in the style of 80s synth-pop / a film score / Japanese city pop`; fusion `A mix of trap and orchestral`, `Folk-punk`. **Compliance:** don't name famous artists; describe the trait instead (`a soaring vocal style reminiscent of power-pop divas`).

---

## Assembly method (4 passes)

1. **骨架** structure + genre: `[Intro][Verse][Chorus], 80s Synth-pop`
2. **皮肤** mood: `Nostalgic and dreamy, for a late-night drive`
3. **衣服** instruments + vocals: `led by a classic synthesizer bassline and electronic drums, with breathy female vocals`
4. **点缀** effects: `lush reverb, subtle tape saturation`

Combined:
```
[Verse][80s Synth-pop, nostalgic and dreamy, for a late-night drive, led by a classic synthesizer bassline and electronic drums, with breathy female vocals, lush reverb, subtle tape saturation]
```

**Hard-code vs leave-open:** explicit when required (`male rap vocals`); broad when you want latitude (`keyboard melody`, `percussion`). **Length:** 30–60 words. Cut contradictions; simpler often wins. **Language:** Chinese for 国风/动感流行/苦情/DJ (better 咬字); English for global electronic terms; front-load the most important word.

---

## Sectional-prompt format (worked shape)

```
[Verse 1][soft piano intro, clean and intimate vocal delivery, sparse instrumentation]
<lyric line>
<lyric line>

[Chorus][driving pop-rock drum beat enters, signature string section swells, powerful layered lead vocals, building emotional intensity]
<lyric line>
```
Meta tags are case-insensitive. Blank line between sections. Use `()` for ad-libs/旁白. 4–8 lyric lines per section generates best.

---

## 8 copy-ready templates (adapt, don't ship verbatim)

These mirror the official template set; trim freely (often shorter = better).

1. **流行情歌 Pop Ballad** — `[Intro][Soft piano arpeggios only, gentle reverb, distant rain fading in]` → build to `[Chorus][full band, lush strings swell, powerful female vocals with layered harmonies, driving drums, wide stereo]`. Slow, intimate→epic.
2. **嘻哈/陷阱 Trap** — `[Intro][Dark Trap, warped vinyl crackle, distant siren, deep sub-bass, eerie piano loop, no drums]` → `[Chorus][Aggressive Trap, distorted 808 hits, fast hi-hats, snare rolls, eerie synth, powerful male rap with layered ad-libs]`.
3. **EDM** — `[Intro][Progressive House, ocean-wave SFX, soft synth pad, 4/4 kick fades in, no bass]` → `[Build-Up][white-noise riser, kick doubles, snare rolls, final bar silence]` → `[Drop]`.
4. **唯美抒情国风** — `Mandopop, Chinese Style, Female Vocal, Guzheng + Piano, Soft Strings, Pentatonic, Mid-tempo, Elegant, Nostalgic`.
5. **宏大侠气国风** — `Epic Wuxia, Grand Orchestral, Dizi, Pipa, Powerful Chinese Drums, Heroic, Cinematic, Pentatonic`.
6. **禅意空灵 (纯音乐/冥想/ambient base)** — `Instrumental, Zen, Guqin solo, Xiao, Minimalist, Ethereal, Deep Reverb, Atmospheric, Peaceful, Slow Tempo, ~60 BPM, loopable`.
7. **新国风电子** — `Guofeng Trap, Aggressive Pipa Plucking, Heavy 808, Hip-hop Beat, Oriental Synth, Dark, High Energy, Fusion`.
8. **氛围都市 R&B** — `breathy female alto, G-minor atmospheric Mandopop R&B, reverbed clean electric guitar, simple electronic drums, deep synth bass, atmospheric synth pads, lyrical piano, slow tempo, lo-fi texture`.

For genre-specific templates with full structured (sectional) examples — including 禅意/ambient build — see `references/genres.md`.
