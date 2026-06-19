# 妙响 (MUSE SONG) AI Music Skill

A [Claude Skill](https://www.anthropic.com/news/skills) that encodes the music-creation methodology for **妙响 (MUSE SONG)** — the AI music creation + distribution platform of **汽水音乐 / 抖音音乐创作实验室**.

Once installed, Claude can help you write music-generation prompts, pick and fuse genres, write lyrics and hooks, choose a generation model, troubleshoot AI output, and optimize a track for 汽水 cold-start traffic — without you having to paste reference material each time.

---

## ⚠️ Source & disclaimer (read first)

This is an **unofficial, community study aid**. Its content is **distilled and rewritten** from 妙响 / 抖音音乐 (ByteDance) official creator knowledge-base material. It is **not** a verbatim copy of the official docs, and it is **not affiliated with, endorsed by, or maintained by** ByteDance, 抖音, 汽水音乐, or 妙响.

- All trademarks (妙响, MUSE SONG, 汽水音乐, 抖音, Sway, SeedMusic, etc.) belong to their respective owners.
- The methodology, formulas, and parameter references summarized here originate from the official knowledge base; this repo reorganizes them for learning convenience.
- If you are a rights holder and want this taken down or adjusted, please open an issue.
- **Time-sensitivity:** based on knowledge-base material as of **2026-06**. Model lineups, platform features, and traffic rules change frequently and may be out of date. Always verify against the current official docs.

Use at your own discretion. Nothing here overrides the platform's terms of service or any agreement you have signed.

---

## What's inside

```
skill/miaoxiang-music/
├── SKILL.md                        # overview, task routing, master prompt formula, the 7 dimensions
└── references/
    ├── prompt-engineering.md       # full 7-dimension vocab, assembly method, 8 templates
    ├── genres.md                   # per-genre formulas, BPM ranges, templates (incl. ambient/梦核 BGM)
    ├── lyrics.md                   # structure, rhyme, imagery, 金句/hook formulas, 诗词 句式
    ├── distribution.md             # 汽水 cold-start: the 5 metrics + tactics, naming, account ops
    └── platform.md                 # features, the model lineup, troubleshooting, external tools

dist/
└── miaoxiang-music.skill           # packaged, ready-to-install build
```

## Install

**Option A — use the prebuilt package (easiest)**
1. Download [`dist/miaoxiang-music.skill`](dist/miaoxiang-music.skill).
2. In Claude (claude.ai or the desktop app): **Settings → Capabilities/Skills → upload** the `.skill` file. (In Claude Code, place the unpacked skill folder in your skills directory.)

**Option B — build it yourself from source**
```bash
# zip the skill folder so the archive root is the skill directory:
cd skill
zip -r ../miaoxiang-music.skill miaoxiang-music
```
Then upload the resulting `.skill` as in Option A.

## How it triggers

You don't need to name 妙响. The skill activates when you ask Claude to:
- write a music-generation prompt (提示词 / structured / 分段)
- pick or fuse a 曲风 (国风/民族国韵, EDM/电子, 动感流行, Rap/嘻哈, 禅意/ambient/梦核 BGM)
- write or refine lyrics, hooks (金句), rhyme (押韵), or 诗词 句式
- choose a generation model (Sway, SeedMusic, Mureka, MiniMax, TemPolor, Sodance, 音潮)
- troubleshoot AI output (唱错字 / 咬字 / 乱发挥)
- optimize a track for 汽水 cold-start (冷启 / 起量 / 完播率 / 30s跳出率 / 被选用 / BGM)

…even if you only describe the outcome (e.g. "help me make a creepy ambient BGM", "write me a viral hook").

## Contributing

Issues and PRs welcome — especially corrections when the platform's models, features, or rules change. Please edit the **source files** under `skill/miaoxiang-music/`, not the packaged `.skill`. After changes, repackage with the command in Option B (and bump the date in the disclaimer).

## License

[MIT](LICENSE) for the **structure, wording, and organization** of this repository. This license does not grant rights to any third-party trademarks or to the underlying official material it summarizes.
