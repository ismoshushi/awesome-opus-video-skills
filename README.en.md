# awesome-opus-video-skills

[中文说明](README.md)

A curated index of **open-source, installable Agent skills that make videos by writing code** — the workflow Claude Opus 5.5 is actually good at.

**The one idea behind this list:** Opus 5.5 does not render pixels natively. It *writes rendering code* — Canvas, Remotion, p5.js, GSAP — drives a headless browser frame by frame, and stitches the result with ffmpeg. The skills collected here package that pipeline so you can install one and just say: "make me a 60-second video about X".

This repo only **links** to open-source projects — no third-party source code is re-hosted. Every entry lists: what it does, render stack, install command, license, and whether it was built specifically for Opus 5.5.

## ⚡ Quick overview — all 39 skills

Categories: **①** Code-to-video · **②** Product videos & footage editing · **③** Watch videos / video-to-skill · **④** External video-model callers

| # | Skill | One-liner | ⭐ | License | 5.5? |
| --- | --- | --- | --- | --- | --- |
| ① | [klsoen/opus-js-animations](https://github.com/klsoen/opus-js-animations) | Director-style: brief → voiceover → treatment → frame-exact MP4 rendered in JS | 15 | MIT | ✅ |
| ① | [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | Cinematic Remotion product promos: 152 shot recipe cards + production template | 9,949 | Apache-2.0 | — |
| ① | [bestagentkits/motion-video-skill](https://github.com/bestagentkits/motion-video-skill) | Beat-synced 1080p HyperFrames (HTML+GSAP) with AI voice-over & karaoke captions | 103 | MIT | — |
| ① | [haidrrrry/claude-remotion-skill](https://github.com/haidrrrry/claude-remotion-skill) | Teaches Claude Remotion motion graphics: editing, B-roll, captions, sound | 225 | MIT | — |
| ① | [JohnHeibel/ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | Hand-painted cartoon kit: p5.js + the Clawd character + 31 acted emotions | 589 | MIT | ✅ |
| ① | [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) | Motion-graphics B-roll pack for Claude Code / Codex | 338 | MIT | — |
| ① | [Changroro/code-video](https://github.com/Changroro/code-video) | Researches a topic, then renders a hand-drawn + 8-bit promo video | 44 | MIT | ✅ |
| ① | [JagZ999/explainer-video](https://github.com/JagZ999/explainer-video) | Product explainers with voiceover, music & synced SFX | 2 | MIT | — |
| ① | [misbahsy/claude-horizon-animation](https://github.com/misbahsy/claude-horizon-animation) | Recreates the Opus 5.5 announcement-style animation | 4 | ⚠️ Unstated | ✅ |
| ① | [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | Hand-painted watercolor animation + kinetic typography, two skills, 100% code-generated | 33 | MIT | ✅ |
| ① | [howseen-ai/claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | Pure-code motion: deterministic seek(t) + beat-sync, with a frame-by-frame remake mode | 105 | MIT | ✅ |
| ① | [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | One music track + one prompt → motion-graphics MV (Opus 5.5 plugin) | 69 | MIT | ✅ |
| ① | [echris6/motion-video-kit](https://github.com/echris6/motion-video-kit) | Business-ad skill kit: independent critic loop + methodology from 28 launch films | 72 | MIT | — |
| ① | [Kimeur/motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) | 8 skills in one: kinetic type / 3D / pixel / particles / App UI loop shorts | 4 | MIT | — |
| ① | [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple-style launch films: __seek(t) + headless Chrome + ElevenLabs | 1 | MIT | ✅ |
| ① | [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | Disciplined motion pipeline: automated QA + original score | 1 | MIT | — |
| ① | [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | Code shorts with live annotated preview + blind-read QC | 0 | MIT | — |
| ① | [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | 6-step pipeline: HyperFrames + GSAP + Whisper word-level alignment | 3 | MIT | ✅ |
| ① | [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | Paper-collage vertical videos from HyperFrames templates | 3 | MIT | — |
| ① | [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | Reads your link for brand → renders film + original synth soundtrack | 13 | MIT | — |
| ① | [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | Your narration + real assets → 6 styles, 20–60s promos | 12 | MIT | ✅ |
| ① | [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | Talking-head choreography: HTML/JS motion + Chromium frame-by-frame + ffmpeg | 18 | MIT | — |
| ① | [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | HTML slides + TTS + ASR round-trip check → narrated MP4 (zh/en/yue) | 1 | MIT | — |
| ② | [browser-use/video-use](https://github.com/browser-use/video-use) | Edit videos with coding agents: cuts, captions, color, overlaid animation | 27,657 | MIT | — |
| ② | [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | Motion-design fundamentals (timing/type/color/composition) + Remotion engine | 39 | MIT | — |
| ② | [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram / intro / outro — turn episodes into channel branding | 4 | MIT | — |
| ② | [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | Conversational AI editor: Agent Skills + MCP + Remotion, multi-track timeline | 2,056 | AGPL-3.0 | — |
| ② | [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | Talking-head full-screen stage packaging: Remotion + staged review gates | 1 | MIT | — |
| ② | [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | Talking-head motion base + dozens of shot templates: transparent layers + ffmpeg compositing | 0 | Apache-2.0 | — |
| ② | [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | Voice memo → 1080×1920 animated Short: word-level captions + auto score | 16 | MIT | — |
| ③ | [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | Teaches your AI to watch videos: learn, absorb, imitate, give feedback | 70 | MIT | — |
| ③ | [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | Turns videos and courses into evidence-grounded Agent Skills | 31 | MIT | — |
| ③ | [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | ffmpeg + local Whisper so Claude understands local videos (offline) | 9 | ⚠️ Unstated | — |
| ③ | [tomascupr/reelql](https://github.com/tomascupr/reelql) | Video link in → one typed JSON: chapters/people/brands/emotion arc/transcript | 28 | MIT | — |
| ④ | [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills + exact Seedance/Kling/Veo prompt syntax | 455 | CC-BY-4.0 | — |
| ④ | [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 video models + self-improving QC loop | 6 | MIT | — |
| ④ | [scenario-labs/skills](https://github.com/scenario-labs/skills) | Scenario MCP: on-demand model picking for image/video/audio/3D + Blender/Maya/Unreal expert skills | 751 | MIT | — |
| ④ | [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Smart routing across 7 providers: OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D | 2 | Apache-2.0 | — |
| ④ | [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | 11 skills: full AI short-drama pipeline (script → storyboard → prompts → film) | 2,395 | MIT | — |

> "5.5?" criteria (verified per-repo from READMEs/descriptions): **✅** = explicitly names Opus 5.5; **—** = not explicitly named (mostly generic Claude skills — generic means compatible with 5.5). **⚠️** = no standard SPDX license badge found; confirm before final inclusion. **⭐** = star snapshot taken 2026-09-30, for rough quality screening only.

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
| [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | Two skills — hand-painted watercolor animation (character acting, karaoke captions) + kinetic typography (WebGL layers); everything generated in code, no image/audio models。<br>双 skill：手绘水彩动画（含角色表演、卡拉 OK 字幕）+ kinetic typography（WebGL 图层），全代码生成、无图像/音频模型。 | p5.js/p5.brush + three.js/WebGL + headless Chrome + ffmpeg（音乐代码合成） | `/plugin marketplace add tuzhechen2005/opus-video-skills` | MIT | **Yes** |
| [howseen-ai/claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | Pure-code motion design: deterministic seek(t) rendering, beat-sync, per-peak SFX, plus a remake mode that recreates any launch film frame by frame。<br>纯代码动效：seek(t) 确定性渲染、节拍同步、逐峰音效，附带 remake 模式（逐帧复刻任意发布片）。 | HTML + Playwright + ffmpeg（无 Remotion 许可依赖） | `cp -r skill/motion-design ~/.claude/skills/` | MIT | **Yes** |
| [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | One music track + one prompt → high-quality motion-graphics MV; 6 finished videos already on YouTube。<br>一条音乐 + 一句 prompt → 高质量 motion graphics MV，已有 6 支 YouTube 成片。 | Node/P5JS 动画 + FAL.ai（图像/动画/音频）+ Python 混音；⚠ 需 FAL API key，约 $30 + 3M tokens / 3 分钟歌 | `/plugin marketplace add makevoid/motion-graphics-music-video-skill` | MIT | **Yes** |
| [echris6/motion-video-kit](https://github.com/echris6/motion-video-kit) | Business-ad skill kit: builder≠judge independent critic loop + methodology distilled from 28 SaaS launch films + Three.js product realism。<br>商务广告 skill kit：builder≠judge 的独立评审循环 + 28 部 SaaS 发布片方法论 + Three.js 产品写实。 | HTML/GSAP + Three.js + ffmpeg，HyperFrames 可选 | `cp -r motion-video-kit/business-motion-film ~/.claude/skills/` | MIT | — |
| [Kimeur/motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) | 8 skills in one kit: kinetic type / shapes / cartoon / 3D / charts / pixel / particles / app UI, as looping shorts。<br>8 个 skill 一套：kinetic type / shapes / cartoon / 3D / charts / pixel / particles / app UI，循环短片。 | 单 HTML 文件 seek(t) + 逐帧渲染 + 真实动态模糊 | `/plugin marketplace add Kimeur/motion-launch-videos` | MIT | — |
| [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple-style launch films: visuals and audio share one timeline.json so they never drift。<br>Apple 风产品发布片：画面与音频共用 timeline.json 永不漂移。 | __seek(t) + headless Chrome + ffmpeg；ElevenLabs 音乐/配音/音效 | `npx skills add Dwite/launch-film -g` | MIT | **Yes** |
| [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | Disciplined pipeline: forced pre-read rules + automated QA (frozen frames / text collisions / non-determinism, qa.mjs) + original score。<br>纪律化 pipeline：强制读前置规则 + 自动 QA（冻帧/文字碰撞/非确定性检测，qa.mjs）+ 自创配乐。 | HTML 模板 + headless render + ffmpeg | `npx skills add Lob0Garou/opus-visual-motion-engine` | MIT | — |
| [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | Code-rendered shorts: live annotatable preview + blind-read QC (a fresh agent must restate the argument from still frames)。<br>代码短片：可标注实时预览 + 盲读质检（fresh agent 只看静帧复述论点）。 | HTML + Playwright + ffmpeg；音乐先行、按小节剪辑 | `/plugin marketplace add wcfcarolina13/motion-studio` | MIT | — |
| [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | 6-step universal pipeline: research → storyboard → TTS → Whisper word-level alignment → GSAP build → headless render。<br>6 步通用管线：调研 → 分镜 → TTS → Whisper 词级对齐 → GSAP 构建 → 无头渲染。 | HyperFrames + HTML/SVG/GSAP + whisper.cpp | `npx skills add siyuanfeng636-cpu/agentic-motion-graphics` | MIT | **Yes** |
| [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | Paper-collage vertical videos: torn-paper typewriter captions, photo stickers, stop-motion feel。<br>纸拼贴风竖屏视频：撕纸条打字机字幕、照片贴纸、定格感。 | HyperFrames（纯 HTML 逐帧）+ ffmpeg | `/plugin marketplace add rafiimanggala/paper-collage-skill` | MIT | — |
| [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | Reads a link to extract the brand (real UI/colors/fonts) → writes a treatment → renders film + original score from a homegrown synth。<br>给链接读品牌（真实 UI/配色/字体）→ 写导演阐述 → 出片 + 自研合成器原创配乐。 | headless Chrome + HTML + 自研 synth（80 音色）+ ffmpeg | `npx skills add Mort1d/motion-graphics-skills` | MIT | — |
| [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | Your narration + real assets (covers/screenshots used as-is) → 6 styles, 20–60s promos。<br>自己的旁白 + 真实素材（封面/截图原样使用）→ 6 种风格 20–60 秒 promo。 | 代码渲染 + ffmpeg，本地出片 | `npx skills add axtonliu/video-illustrator` | MIT | **Yes** |
| [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | Talking-head choreography: titles/cards/app windows/bilingual captions + Chromium frame-by-frame MP4 export; ⚠ some templates still being uploaded。<br>真人口播编排：标题/卡片/软件窗口/双语字幕 + Chromium 逐帧导出 MP4；⚠ 部分模板仍在上传中。 | HTML/JS + Chromium + ffmpeg | `git clone https://github.com/adunext/adu-motion-video.git ~/.claude/skills/adu-motion-video` | MIT | — |
| [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | Outline/script → narrated MP4: 13 themes, 17 layouts, TTS + ASR round-trip verification (zh/en/yue); built for MiniMax Code。<br>大纲/脚本 → 口播 MP4：13 套主题、17 种版式，TTS + ASR 回译校验配音（中/英/粤）；为 MiniMax Code 构建。 | HTML slides + TTS + Whisper 校验 + ffmpeg | 见原仓库 README（为 MiniMax Code 构建） | MIT | — |

\* 页面未显示标准许可证标识，可能是自定义许可证；收录前需到原仓库确认。Page shows no standard SPDX license badge — confirm in the source repo.

> The makevoid entry generates part of its audio/assets via FAL — bring your own API key (~$30 + 3M tokens per 3-minute song); everything else renders locally from code.

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
| [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | Open-source ChatCut alternative: conversational AI editor that keeps a professional multi-track timeline editable。<br>开源 ChatCut 替代：对话式 AI 剪辑器，专业多轨时间线保持可编辑。 | Agent Skills + MCP + Remotion 渲染 | `npx skills add 0xsline/OpenChatCut` | AGPL-3.0 | — |
| [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | Talking-head → full-screen visual stage packaging: semantic-driven animation + staged review gates (A→D)。<br>口播 → 全屏视觉舞台包装：语义驱动动画 + 分阶段审核（Gate A→D）。 | Remotion | clone 后 `npm ci`，拷入 skills 目录 | MIT | — |
| [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | Talking-head motion base: reads storyboard JSON → transparent overlay layers → ffmpeg layered compositing + QA gate。<br>口播动效底座：读分镜 JSON → 透明动效叠层 → ffmpeg 分层合成 + QA 门禁。 | 浏览器内渲染内核 + ffmpeg | 见原仓库 README | Apache-2.0 | — |
| [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | Voice memo → 1080×1920 animated Short: word-level captions, kinetic typography, auto score。<br>语音备忘录 → 1080×1920 动画 Short：逐词字幕、kinetic typography、自动配乐。 | 代码渲染 + ffmpeg，全本地 | 见原仓库 README | MIT | — |

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
| [tomascupr/reelql](https://github.com/tomascupr/reelql) | Any video link → one typed JSON: summary / chapters / people / brands / emotion arc / transcript。<br>任意视频链接 → 一份 typed JSON：摘要/章节/人物/品牌/情感弧线/逐字稿。 | 视频理解 API + skill | 见原仓库 README（.claude-plugin） | MIT | — |

</details>

### ④ External video-model callers (kept separate on purpose)

<details>
<summary><b>Expand 5 entries</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills — Murch-style dramaturgy, blocking, montage + exact prompt syntax for Seedance 2.5 / Kling 3.0 / Veo 3.1。<br>AI 导演技能：Murch 剪辑理论、走位、蒙太奇 + Seedance 2.5 / Kling 3.0 / Veo 3.1 精确提示词语法。 | 外部视频模型 API（提示词语法库） | `npx skills add smixs/visual-skills` | CC-BY-4.0 | — |
| [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 models (Seedance 2.0, Kling, Wan, Veo, OmniHuman) with a self-improving QC loop。<br>跨 6 个模型端到端出片，带自我改进的质量控制环。 | 外部视频模型 API + ffmpeg 后期 | `npx skills add 0xadvait/ai-video-skill` | MIT | — |
| [scenario-labs/skills](https://github.com/scenario-labs/skills) | Scenario MCP: smart model picking for image/video/audio/3D + expert skill teams that drive Blender/Maya/Unreal。<br>Scenario MCP：智能选模型出图/视频/音频/3D + 驱动 Blender/Maya/Unreal 的专家 skill 团队。 | Scenario MCP + DCC 软件 | 见原仓库 README | MIT | — |
| [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Smart routing across 7 providers (OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D) with cost gating。<br>七家供应商智能路由（OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D），成本门控。 | 外部模型 API | 见原仓库 README | Apache-2.0 | — |
| [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | 11 skills: full AI short-drama pipeline (source analysis → episodic scripts → storyboard → prompts → film → review)。<br>11 个 skill：AI 短剧/漫剧全流程（原著分析 → 分集剧本 → 分镜 → 提示词 → 成片 → 审查）。 | 视频生成模型 + 剪辑 | 见原仓库 README | MIT | — |

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
- [jacobbubu/claude-opus-5-5-js-animation-research](https://github.com/jacobbubu/claude-opus-5-5-js-animation-research) — 30 verified Opus 5.5 browser-animation cases, ranked by X views (go here for implementation deep-dives)

The first two index **outputs and workflows**; the last two are **prompt collections and technical casebooks**. This repo indexes **installable skills** — different jobs.

## Contributing

PRs welcome — read [CONTRIBUTING.md](CONTRIBUTING.md). Short version: public repo, installable skill (`SKILL.md` or plugin), produces or processes video, license stated, **links only**; new entries must update the tables in **both** `README.md` and `README.en.md`.

## License & disclaimer

- This index is [MIT](LICENSE) licensed; it contains no third-party code, only links and short descriptions.
- Not affiliated with or endorsed by Anthropic. Claude and Opus are trademarks of Anthropic PBC.
- Each listed project keeps its own license — the source repo is always authoritative.
