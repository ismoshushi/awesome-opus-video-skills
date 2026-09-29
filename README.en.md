# awesome-opus-video-skills

[中文说明](README.md)

A curated index of **open-source, installable Agent skills that make videos by writing code** — the workflow Claude Opus 5.5 is actually good at.

**The one idea behind this list:** Opus 5.5 does not render pixels natively. It *writes rendering code* — Canvas, Remotion, p5.js, GSAP — drives a headless browser frame by frame, and stitches the result with ffmpeg. The skills collected here package that pipeline so you can install one and just say: "make me a 60-second video about X".

This repo only **links** to open-source projects — no third-party source code is re-hosted. Every entry lists: what it does, render stack, install command, license, and whether it was built specifically for Opus 5.5.

## ⚡ Quick overview — all 39 skills

Categories: **①** Code-to-video · **②** Product videos & footage editing · **③** Watch videos / video-to-skill · **④** External video-model callers

| # | Skill | One-liner | License | 5.5? |
| --- | --- | --- | --- | --- |
| ① | [klsoen/opus-js-animations](https://github.com/klsoen/opus-js-animations) | Director-style: brief → voiceover → treatment → frame-exact MP4 rendered in JS | MIT | ✅ |
| ① | [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | Cinematic Remotion product promos: 152 shot recipe cards + production template | Apache-2.0 | — |
| ① | [bestagentkits/motion-video-skill](https://github.com/bestagentkits/motion-video-skill) | Beat-synced 1080p HyperFrames (HTML+GSAP) with AI voice-over & karaoke captions | MIT | — |
| ① | [haidrrrry/claude-remotion-skill](https://github.com/haidrrrry/claude-remotion-skill) | Teaches Claude Remotion motion graphics: editing, B-roll, captions, sound | MIT | — |
| ① | [JohnHeibel/ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | Hand-painted cartoon kit: p5.js + the Clawd character + 31 acted emotions | MIT | ✅ |
| ① | [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) | Motion-graphics B-roll pack for Claude Code / Codex | MIT | — |
| ① | [Changroro/code-video](https://github.com/Changroro/code-video) | Researches a topic, then renders a hand-drawn + 8-bit promo video | MIT | ✅ |
| ① | [JagZ999/explainer-video](https://github.com/JagZ999/explainer-video) | Product explainers with voiceover, music & synced SFX | MIT | — |
| ① | [misbahsy/claude-horizon-animation](https://github.com/misbahsy/claude-horizon-animation) | Recreates the Opus 5.5 announcement-style animation | ⚠️ Unstated | ✅ |
| ① | [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | Built for Opus 5.5: every frame and note generated in code, one skill per style | MIT | ✅ |
| ① | [howseen-ai/claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | Pure-code motion design: HTML + Playwright + ffmpeg, no AE / Remotion license | MIT | ✅ |
| ① | [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | Music track + one prompt → high-quality MG video (Opus 5.5 plugin) | MIT | ✅ |
| ① | [echris6/motion-video-kit](https://github.com/echris6/motion-video-kit) | Premium business-video kit: critic loop + motion principles from 28 launch films | MIT | — |
| ① | [Kimeur/motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) | Brief → looping kinetic-typography launch video (single-file HTML, deterministic) | MIT | — |
| ① | [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple-style launch films: frame-by-frame in code, beat-locked score + voiceover | MIT | ✅ |
| ① | [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | Deterministic seek(t) + automated render QA — works even for text-only models | MIT | — |
| ① | [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | Code-rendered MG films: annotated preview, beat-cut licensed music, blind-read gate | MIT | — |
| ① | [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | Autonomous code-to-video engine: HyperFrames + GSAP + Whisper + TTS | MIT | ✅ |
| ① | [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | DIY paper-collage videos (HyperFrames) | MIT | — |
| ① | [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | Showreel-grade code motion graphics, original soundtrack per video | MIT | — |
| ① | [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | Your narration + real assets + any look → a short film | MIT | ✅ |
| ① | [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | Editable HTML/JS scenes + talking-head layouts, verified local MP4 export | MIT | — |
| ① | [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | Topic/script → narrated MP4: HTML slides + TTS + ASR verification | MIT | — |
| ② | [browser-use/video-use](https://github.com/browser-use/video-use) | Edit videos with coding agents: cuts, captions, color, overlaid animation | MIT | — |
| ② | [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | Motion-design fundamentals (timing/type/color/composition) + Remotion engine | MIT | — |
| ② | [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram / intro / outro — turn episodes into channel branding | MIT | — |
| ② | [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | Local-first conversational video editor: multi-track timeline + MCP + Remotion | AGPL-3.0 | — |
| ② | [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | Talking-head stage-visual packaging: Remotion compositing + review frames | MIT | — |
| ② | [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | Talking-head editing engine: storyboard-driven MG + reusable shot library | Apache-2.0 | — |
| ② | [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | Voice note → animated, sound-designed Short | MIT | — |
| ③ | [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | Teaches your AI to watch videos: learn, absorb, imitate, give feedback | MIT | — |
| ③ | [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | Turns videos and courses into evidence-grounded Agent Skills | MIT | — |
| ③ | [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | ffmpeg + local Whisper so Claude understands local videos (offline) | ⚠️ Unstated | — |
| ③ | [tomascupr/reelql](https://github.com/tomascupr/reelql) | Video link in, typed JSON out — gives your agent eyes | MIT | — |
| ④ | [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills + exact Seedance/Kling/Veo prompt syntax | CC-BY-4.0 | — |
| ④ | [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 video models + self-improving QC loop | MIT | — |
| ④ | [scenario-labs/skills](https://github.com/scenario-labs/skills) | Production images/video/audio/3D: model picking + price-before-spend | MIT | — |
| ④ | [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Universal visual generation across model APIs + smart cost gating | Apache-2.0 | — |
| ④ | [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | AI short-drama kit: script → storyboard → prompts | MIT | — |

> "5.5?" criteria (first batch verified per-repo on 2026-09-27, new batch on 2026-09-29, from each repo's README/description): **✅** = explicitly names Opus 5.5; **—** = not explicitly named (mostly generic Claude skills — generic means compatible with 5.5). **⚠️** = no standard SPDX license badge found; confirm before final inclusion.

## Category details (click to expand)

### ① Code-to-video — the core Opus 5.5 workflow

<details>
<summary><b>Expand 23 entries: what / stack / install / license</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [klsoen/opus-js-animations](https://github.com/klsoen/opus-js-animations) | Director-style flow: brief → voiceover → treatment → frame-exact MP4, rendered in JavaScript。<br>导演式出片：brief → 配音 → 导演阐述 → JS 渲染帧级精确 MP4。 | JS + Chrome 逐帧渲染 + ffmpeg，AI 配音 | `npx skills add klsoen/opus-js-animations` | MIT | **Yes** |
| [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | Cinematic product promos in Remotion: 152 shot recipe cards, 209 motion previews, production-ready template。<br>Remotion 电影感产品宣传片：152 张镜头配方卡、209 个动效预览、生产级模板。 | Remotion | `npx skills add Vincentwei1021/video-shotcraft` | Apache-2.0 | — |
| [bestagentkits/motion-video-skill](https://github.com/bestagentkits/motion-video-skill) | Beat-synced 1080p motion graphics in HyperFrames (HTML + GSAP) with AI voice-over, karaoke captions, SFX & generated music。<br>HyperFrames + GSAP 出节拍同步 1080p 动态视频：AI 配音、卡拉 OK 字幕、音效与生成音乐。 | HyperFrames（HTML + GSAP）+ ffmpeg | `npx skills add bestagentkits/motion-video-skill` | MIT | — |
| [haidrrrry/claude-remotion-skill](https://github.com/haidrrrry/claude-remotion-skill) | Teaches Claude to build professional motion-graphics videos with Remotion: editing, B-roll, captions, sound。<br>教 Claude 用 Remotion 做专业动态图形：剪辑、B-roll、字幕、配乐。 | Remotion + ffmpeg | 见原仓库 README（skill 在子目录） | MIT | — |
| [JohnHeibel/ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | Starter kit for hand-painted cartoons: p5.js + p5.brush, the Clawd character, 31 acted emotions。<br>手绘动画底板：p5.js + p5.brush、Clawd 角色、31 种表演情绪。 | p5.js（p5.brush）+ Playwright + ffmpeg | 见原仓库 README | MIT | **Yes** |
| [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) | Motion-graphics skill pack for Claude Code / Codex — adds MG B-roll to your footage。<br>Claude Code / Codex 运动图形技能包：给成片加 MG B-roll。 | Playwright + ffmpeg | 见原仓库 README（多 skill 子目录） | MIT | — |
| [Changroro/code-video](https://github.com/Changroro/code-video) | Researches a topic, then renders a hand-drawn + 8-bit promo video (MP4)。<br>调研主题后渲染手绘 + 8-bit 风格宣传短片（MP4）。 | 代码逐帧绘制 + ffmpeg | `npx skills add Changroro/code-video` | MIT | **Yes** |
| [JagZ999/explainer-video](https://github.com/JagZ999/explainer-video) | Animated product explainer videos with voiceover, music & synced SFX。<br>带配音、音乐与同步音效的产品讲解动画。 | Puppeteer 渲染 + ffmpeg + ElevenLabs | `npx skills add JagZ999/explainer-video` | MIT | — |
| [misbahsy/claude-horizon-animation](https://github.com/misbahsy/claude-horizon-animation) | Recreates the Claude Opus 5.5 announcement-style animation。<br>复刻 Claude Opus 5.5 发布公告风格的动画。 | 浏览器逐帧渲染 + ffmpeg | `npx skills add misbahsy/claude-horizon-animation` | ⚠️ 未标注* | **Yes** |
| [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | Video-making skills built for Claude Opus 5.5 — every frame and note generated in code, one skill per style (hand-painted, kinetic typography, ...)。<br>专为 Opus 5.5 打造的视频技能合集：逐帧逐音符全部用代码生成，一种风格一个 skill（手绘动画、动态字体等）。 | 代码逐帧渲染（多种风格子技能）+ 代码生成音频 | `/plugin marketplace add tuzhechen2005/opus-video-skills`（plugin + skills 双形态） | MIT | **Yes** |
| [howseen-ai/claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | Motion design videos in pure code: HTML + Playwright + ffmpeg — no After Effects, no Remotion license。<br>纯代码做运动设计视频：HTML + Playwright + ffmpeg，不需要 After Effects、不买 Remotion 授权。 | HTML + Playwright + ffmpeg | `npx skills add howseen-ai/claude-motion-design` | MIT | **Yes** |
| [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | Opus 5.5 plugin: high-quality motion graphics videos from just a music track and a prompt。<br>只给一段音乐 + 一句提示词，生成高品质运动图形视频（Opus 5.5 plugin）。 | 代码渲染 MG + ffmpeg（部分素材走 FAL，需 API key） | `/plugin marketplace add makevoid/motion-graphics-music-video-skill` | MIT | **Yes** |
| [echris6/motion-video-kit](https://github.com/echris6/motion-video-kit) | Premium AI-assisted business videos: independent critic loop, motion principles from 28 launch films, quality bar, sound design, Three.js patterns。<br>商业级视频技能包：独立评审环、28 部 launch film 提炼的运动原则、质量红线、声音设计与 Three.js 模式。 | Three.js + 代码渲染 | `npx skills add echris6/motion-video-kit` | MIT | — |
| [Kimeur/motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) | Turn a short brief into a looping kinetic-typography launch video: one self-contained HTML file, pure seek(t), closed-form springs, per-glyph motion。<br>一段 brief 变循环播放的动态字体 launch 视频：单文件 HTML、纯 seek(t) 确定性渲染、逐字形弹簧动效。 | 单文件 HTML（closed-form springs）+ 逐帧录制 | `/plugin marketplace add Kimeur/motion-launch-videos`（plugin + skill 双形态） | MIT | — |
| [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple-style product launch films rendered frame by frame in code, cut to a beat-locked score with voiceover and sound。<br>Apple 风格产品发布片：代码逐帧渲染，卡点配乐 + 配音音效。 | 代码逐帧渲染 + 卡点配乐 + TTS | `npx skills add Dwite/launch-film` | MIT | **Yes** |
| [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | Disciplined pipeline for motion graphics, code-rendered video and UI — deterministic seek(t), automated render QA (works for text-only models), MP4 export。<br>纪律化流水线：确定性 seek(t) + 自动渲染质检，纯文本模型也能稳定出 MP4。 | 确定性 seek(t) 渲染 + 自动 QA + MP4 导出 | `npx skills add Lob0Garou/opus-visual-motion-engine` | MIT | — |
| [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | Code-rendered motion-graphics films with live annotated preview, licensed music cut to the beat, recorded foley, and a blind-read gate。<br>代码渲染 MG 影片：实时标注预览、卡点授权音乐、实录拟音、盲听质检门。 | 代码渲染 + 授权音乐/拟音 | `/plugin marketplace add wcfcarolina13/motion-studio` | MIT | — |
| [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | Autonomous code-to-video & motion-graphics engine (Claude Code & Opus 5.5): HyperFrames, GSAP, Whisper, TTS。<br>自主 Code-to-Video 与运动图形引擎（Opus 5.5）：HyperFrames + GSAP + Whisper + TTS 全自动出片。 | HyperFrames + GSAP + Whisper + TTS | `npx skills add siyuanfeng636-cpu/agentic-motion-graphics` | MIT | **Yes** |
| [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | DIY paper collage videos in HyperFrames。<br>DIY 纸拼贴风视频（HyperFrames）。 | HyperFrames | `npx skills add rafiimanggala/paper-collage-skill` | MIT | — |
| [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | Showreel-grade motion graphics from code, with an original soundtrack for every video; works with Claude Code, Codex, Cursor and other agents。<br>showreel 级代码运动图形，每条视频配原创配乐；支持 Claude Code / Codex / Cursor 等多 Agent。 | 代码渲染 + 原创配乐 | `npx skills add Mort1d/motion-graphics-skills` | MIT | — |
| [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | Your voice, your assets, any look you choose — turns your narration and real assets into a short film。<br>你的旁白 + 你的素材 + 任选画风，合成一支短片。 | 旁白驱动 + 素材合成代码渲染 | `npx skills add axtonliu/video-illustrator` | MIT | **Yes** |
| [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | Editable HTML/JS scenes, talking-head layouts, captions, audio and verified local MP4 export。<br>可编辑 HTML/JS 场景 + 口播版式 + 字幕音频，本地导出并逐项校验 MP4。 | HTML/JS 场景 + 本地 MP4 导出校验 | `npx skills add adunext/adu-motion-video` | MIT | — |
| [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | Turn a topic, outline, or script into a narrated MP4: HTML slides + staged animations + TTS voiceover + subtitles + ASR verification。<br>主题/大纲/脚本 → 带旁白 MP4：HTML 幻灯片 + 分段动画 + TTS 配音 + 字幕 + ASR 校验。 | HTML 幻灯片 + TTS + ASR 校验 | `npx skills add Wzdhehe/html2video-for-mcode` | MIT | — |

\* 页面未显示标准许可证标识，可能是自定义许可证；收录前需到原仓库确认。Page shows no standard SPDX license badge — confirm in the source repo.

> The makevoid entry generates part of its audio/assets via FAL — bring your own API key (~$30 per video); everything else renders locally from code.

</details>

### ② Product videos & footage editing

<details>
<summary><b>Expand 7 entries</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [browser-use/video-use](https://github.com/browser-use/video-use) | Edit videos with coding agents — structural cuts, captions, color, overlaid animation。<br>用编码 Agent 剪成片：结构精剪、字幕、调色、叠加动画。 | ffmpeg + Remotion / HyperFrames 叠加 + TTS | `npx skills add browser-use/video-use` | MIT | — |
| [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | Motion-design fundamentals (timing, typography, color, composition) + Remotion engine as installable skills。<br>运动设计基础（节奏、字体、色彩、构图）+ Remotion 引擎，做成可安装技能。 | Remotion | `npx skills add iart-ai/motion-design-skills` | MIT | — |
| [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram + YouTube intro/outro skills — turn every episode into channel branding。<br>Audiogram / YouTube intro / outro：把每期节目变成频道包装件。 | 模板化运动图形 + 旁白 | `npx skills add iart-ai/youtube-video-skills` | MIT | — |
| [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | Open-source, local-first conversational AI video editor: professional multi-track timeline, Agent Skills, MCP integration, Remotion rendering。<br>开源、本地优先的对话式视频编辑器：专业多轨时间线 + Agent Skills + MCP + Remotion 渲染。 | 多轨时间线 + Remotion 渲染 | 见原仓库 README（应用形态，内嵌 skill） | AGPL-3.0 | — |
| [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | Talking-head full-screen stage visual packaging: Remotion compositing, plan approval, review frames and final-output verification。<br>真人口播全屏舞台视觉包装 Skill：Remotion 合成、方案审批、审核帧与成片验证。 | Remotion 合成 + 审批/审核帧流程 | `npx skills add cytxnyu/chuanyuntian-auto-edit-pro` | MIT | — |
| [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | Talking-head editing & packaging engine: storyboard-driven motion graphics, reusable shot library, director skill (Claude Code / Codex)。<br>口播视频剪辑与包装引擎：分镜驱动运动图形 + 可复用镜头库 + 导演 Skill。 | 分镜驱动 MG + 镜头库 | `npx skills add xiaolu-ai26/xiaolu-motion` | Apache-2.0 | — |
| [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | Turn a voice note into an animated, sound-designed Short。<br>一条语音便签 → 带动画与音效设计的竖屏短视频。 | 代码动画 + 音效设计 | `npx skills add Dancan254/voiceover-video-skill` | MIT | — |

</details>

### ③ Watch videos / video-to-skill (adjacent)

<details>
<summary><b>Expand 4 entries</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | Teaches your AI to watch videos — learn, absorb, imitate, or give visual feedback。<br>教 AI「看」视频：学习、吸收、复刻，或像真人一样给视觉反馈。 | 多模态视觉 + ffmpeg 抽帧 | `npx skills add Newuxtreme/watch-video-skill` | MIT | — |
| [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | Turns videos and courses into evidence-grounded Agent Skills。<br>把视频和课程转成有据可查的 Agent Skill。 | ffmpeg 抽帧 / 转写 | `npx skills add Lum1104/video-to-skill` | MIT | — |
| [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | Lets Claude watch & understand local videos via ffmpeg + local Whisper; offline, drops into `~/.claude/skills/`。<br>用 ffmpeg + 本地 Whisper 让 Claude 看懂本地视频，离线可用。 | ffmpeg + 本地 Whisper | `npx skills add Moh4696/claude-video-vision` | ⚠️ 未标注* | — |
| [tomascupr/reelql](https://github.com/tomascupr/reelql) | Give your agent eyes: any video link in, one typed JSON out. A Claude skill + API。<br>给 Agent 装上眼睛：任意视频链接进，一个结构化 JSON 出（skill + API）。 | 视频理解 API（结构化输出） | `/plugin marketplace add tomascupr/reelql` | MIT | — |

</details>

### ④ External video-model callers (kept separate on purpose)

<details>
<summary><b>Expand 5 entries</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills — Murch-style dramaturgy, blocking, montage + exact prompt syntax for Seedance 2.5 / Kling 3.0 / Veo 3.1。<br>AI 导演技能：Murch 剪辑理论、走位、蒙太奇 + Seedance 2.5 / Kling 3.0 / Veo 3.1 精确提示词语法。 | 外部视频模型 API（提示词语法库） | `npx skills add smixs/visual-skills` | CC-BY-4.0 | — |
| [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 models (Seedance 2.0, Kling, Wan, Veo, OmniHuman) with a self-improving QC loop。<br>跨 6 个模型端到端出片，带自我改进的质量控制环。 | 外部视频模型 API + ffmpeg 后期 | `npx skills add 0xadvait/ai-video-skill` | MIT | — |
| [scenario-labs/skills](https://github.com/scenario-labs/skills) | Production-ready images, video, audio and 3D from any AI agent: picks the right model, prices before spending, keeps characters & brands consistent (Scenario MCP)。<br>生产级图/视频/音频/3D 生成：自动选模型、先报价再花、角色与品牌一致性（Scenario MCP）。 | Scenario MCP + 托管模型 API | `npx skills add scenario-labs/skills` | MIT | — |
| [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Universal visual generation skill — images, SVG, video, audio via OpenAI, Gemini, FAL, KIE, HeyGen, ElevenLabs with smart cost gating。<br>通用视觉生成 skill：图/SVG/视频/音频走多家模型，带智能成本闸门。 | OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs API | `npx skills add hectorcanaimero/da-vinci` | Apache-2.0 | — |
| [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | Open-source AI short-drama skills for Claude Code & Codex: script, character assets, storyboard, image/video prompts, review。<br>开源 AI 短剧/漫剧创作 skill 合集：剧本、角色资产、分镜、图/视频提示词、审查。 | 剧本 → 分镜 → 图/视频提示词流水线 | `npx skills add zenstory-ai/drama-skills` | MIT | — |

> Category ④ calls hosted models to generate pixels — a different paradigm from code-to-video, listed separately to avoid confusion.

</details>

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

- [athemeroy/awesome-opus-5-5-videos](https://github.com/athemeroy/awesome-opus-5-5-videos) — a source-linked guide to 1,000+ videos made with Opus 5.5 (go here to *watch*)
- [opusvideo/awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) — Opus 5.5 videos & animations: demos, prompts, workflows (English / 中文)
- [LeaddeOpenLab/awesome-opus-5-5-video-prompts](https://github.com/LeaddeOpenLab/awesome-opus-5-5-video-prompts) — a curated collection of Opus 5.5 video prompts (go here to *copy prompts*)
- [jacobbubu/claude-opus-5-5-js-animation-research](https://github.com/jacobbubu/claude-opus-5-5-js-animation-research) — technical research notes on Opus 5.5 JS animation (go here for implementation deep-dives)

The first two index **outputs and workflows**; the last two are **prompt collections and research notes**. This repo indexes **installable skills** — different jobs.

## Contributing

PRs welcome — read [CONTRIBUTING.md](CONTRIBUTING.md). Short version: public repo, installable skill (`SKILL.md` or plugin), produces or processes video, license stated, **links only**; new entries must update the tables in **both** `README.md` and `README.en.md`.

## License & disclaimer

- This index is [MIT](LICENSE) licensed; it contains no third-party code, only links and short descriptions.
- Not affiliated with or endorsed by Anthropic. Claude and Opus are trademarks of Anthropic PBC.
- Each listed project keeps its own license — the source repo is always authoritative.
