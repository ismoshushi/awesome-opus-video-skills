# awesome-opus-video-skills

A curated index of **open-source, installable Agent skills that make videos by writing code** — the workflow Claude Opus 5.5 is actually good at. [中文说明](README.zh-CN.md)

**The one idea behind this list:** Opus 5.5 does not render pixels natively. It *writes rendering code* — Canvas, Remotion, p5.js, GSAP — drives a headless browser frame by frame, and stitches the result with ffmpeg. The skills collected here package that pipeline so you can install one and just say: "make me a 60-second video about X".

This repo only **links** to open-source projects — no third-party source code is re-hosted. Every entry lists: what it does, render stack, install command, license, and whether it was built specifically for Opus 5.5.

→ Full tables: **[skills.md](skills.md)**

## Categories

1. **Code-to-video** — the core Opus 5.5 workflow: the model writes render code, a browser renders frames, ffmpeg encodes the MP4. Deterministic, re-renderable, no gen-AI flicker.
2. **Product videos & footage editing** — polish existing footage: structural cuts, captions, color, motion-graphics overlays, intros/outros.
3. **Watch videos / video-to-skill** *(adjacent)* — not making videos; making the agent *understand* them, or distilling videos into reusable skills.
4. **External video-model callers** *(kept separate on purpose)* — call hosted text-to-video APIs (Seedance / Kling / Veo style). Useful, but a different paradigm from code-to-video.

## Installing a skill

Most repos here follow the standard skills-CLI convention:

```bash
npx skills add <owner>/<repo>
```

Alternatives:

- copy the skill folder into `~/.claude/skills/`
- plugin-format repos: inside Claude Code, `/plugin marketplace add <owner>/<repo>`, then `/plugin install <plugin-name>`
- if the source repo documents its own install command, that one wins

## Related lists

- [athemeroy/awesome-opus-5-5-videos](https://github.com/athemeroy/awesome-opus-5-5-videos) — a source-linked guide to 1,000+ videos made with Opus 5.5
- [opusvideo/awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) — Opus 5.5 videos & animations: demos, prompts, workflows (English / 中文)

Those lists mostly index **outputs and workflows**; this one indexes **installable skills**. Low overlap, different jobs.

## Contributing

PRs welcome — read [CONTRIBUTING.md](CONTRIBUTING.md) first. Short version: public repo, installable skill (`SKILL.md` or plugin), produces or processes video, license stated, **links only**.

## License & disclaimer

- This index is [MIT](LICENSE) licensed; it contains no third-party code, only links and short descriptions.
- Not affiliated with or endorsed by Anthropic. Claude and Opus are trademarks of Anthropic PBC.
- Each listed project keeps its own license — the source repo is always authoritative.
