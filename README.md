# awesome-opus-video-skills

English: [README.en.md](README.en.md)

一份只收 **开源、可安装的视频类 Agent Skill** 的精选索引——主打 Claude Opus 5.5 真正擅长的出片方式。

**这个列表只讲一件事：** Opus 5.5 出片不是自己画像素，而是**写渲染代码**——Canvas、Remotion、p5.js、GSAP——用无头浏览器逐帧渲染，再用 ffmpeg 合成。这里收的 skill 就是把这条流水线打包好，装上就能说：「给我做一条 60 秒的 XX 视频」。

本仓库只放**链接**，不托管任何第三方源码。每条固定字段：一句话用途、渲染栈、安装命令、许可证、是否专为 Opus 5.5。

## ⚡ 速览全部 39 个 skill

分类：**①** 用代码出片 · **②** 产品片/成片编辑 · **③** 看视频/视频转 skill · **④** 调用外部视频模型

| # | Skill | 一句话用途 | ⭐ | License | 5.5? |
| --- | --- | --- | --- | --- | --- |
| ① | [klsoen/opus-js-animations](https://github.com/klsoen/opus-js-animations) | 导演式出片：brief → 配音 → 导演阐述 → JS 渲染帧级精确 MP4 | 15 | MIT | ✅ |
| ① | [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | Remotion 电影感产品宣传片：152 张镜头配方卡 + 生产级模板 | 9,949 | Apache-2.0 | — |
| ① | [bestagentkits/motion-video-skill](https://github.com/bestagentkits/motion-video-skill) | HyperFrames + GSAP 节拍同步 1080p：AI 配音、卡拉 OK 字幕 | 103 | MIT | — |
| ① | [haidrrrry/claude-remotion-skill](https://github.com/haidrrrry/claude-remotion-skill) | 教 Claude 用 Remotion 做动态图形：剪辑、B-roll、字幕、配乐 | 225 | MIT | — |
| ① | [JohnHeibel/ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | 手绘动画底板：p5.js + Clawd 角色 + 31 种表演情绪 | 589 | MIT | ✅ |
| ① | [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) | 给成片加运动图形 B-roll（Claude Code / Codex） | 338 | MIT | — |
| ① | [Changroro/code-video](https://github.com/Changroro/code-video) | 调研主题后渲染手绘 + 8-bit 宣传短片 | 44 | MIT | ✅ |
| ① | [JagZ999/explainer-video](https://github.com/JagZ999/explainer-video) | 产品讲解动画：配音、音乐、同步音效 | 2 | MIT | — |
| ① | [misbahsy/claude-horizon-animation](https://github.com/misbahsy/claude-horizon-animation) | 复刻 Opus 5.5 发布公告风格动画 | 4 | ⚠️ 未标注 | ✅ |
| ① | [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | 手绘水彩动画 + kinetic typography 双 skill，全代码生成 | 33 | MIT | ✅ |
| ① | [howseen-ai/claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | 纯代码动效：seek(t) 确定性渲染 + 节拍同步，附 remake 复刻模式 | 105 | MIT | ✅ |
| ① | [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | 一条音乐 + 一句 prompt → motion graphics MV（Opus 5.5 plugin） | 69 | MIT | ✅ |
| ① | [echris6/motion-video-kit](https://github.com/echris6/motion-video-kit) | 商务广告 skill kit：独立评审循环 + 28 部发布片方法论 | 72 | MIT | — |
| ① | [Kimeur/motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) | 8 个 skill 一套：kinetic type / 3D / 像素 / 粒子 / App UI 循环短片 | 4 | MIT | — |
| ① | [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple 风产品发布片：__seek(t) + headless Chrome + ElevenLabs | 1 | MIT | ✅ |
| ① | [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | 纪律化 motion pipeline：自动 QA + 自创配乐 | 1 | MIT | — |
| ① | [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | 代码短片 + 可标注实时预览 + 盲读质检 | 0 | MIT | — |
| ① | [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | HyperFrames + GSAP + Whisper 词级对齐的 6 步出片管线 | 3 | MIT | ✅ |
| ① | [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | 纸拼贴风竖屏视频：HyperFrames 模板化出片 | 3 | MIT | — |
| ① | [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | 从链接读品牌 → 出片 + 自研合成器原创配乐 | 13 | MIT | — |
| ① | [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | 自己的旁白 + 真实素材 → 6 种风格 20–60 秒 promo | 12 | MIT | ✅ |
| ① | [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | 真人口播编排：HTML/JS 动效 + Chromium 逐帧 + ffmpeg | 18 | MIT | — |
| ① | [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | HTML 幻灯片 + TTS + ASR 回译校验 → 口播 MP4（中/英/粤） | 1 | MIT | — |
| ② | [browser-use/video-use](https://github.com/browser-use/video-use) | 用编码 Agent 剪成片：精剪、字幕、调色、叠加动画 | 27,657 | MIT | — |
| ② | [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | 运动设计基础（节奏/字体/色彩/构图）+ Remotion 引擎 | 39 | MIT | — |
| ② | [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram / intro / outro 频道包装件 | 4 | MIT | — |
| ② | [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | 对话式 AI 剪辑器：Agent Skills + MCP + Remotion，多轨时间线 | 2,056 | AGPL-3.0 | — |
| ② | [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | 口播全屏视觉舞台包装：Remotion + 分阶段审核 | 1 | MIT | — |
| ② | [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | 口播动效底座 + 几十个镜头库：透明层 + ffmpeg 分层合成 | 0 | Apache-2.0 | — |
| ② | [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | 语音备忘录 → 1080×1920 动画 Short：逐词字幕 + 自动配乐 | 16 | MIT | — |
| ③ | [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | 教 AI「看」视频：学习、吸收、复刻、视觉反馈 | 70 | MIT | — |
| ③ | [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | 把视频和课程转成有据可查的 Agent Skill | 31 | MIT | — |
| ③ | [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | ffmpeg + 本地 Whisper 看懂本地视频（离线可用） | 9 | ⚠️ 未标注 | — |
| ③ | [tomascupr/reelql](https://github.com/tomascupr/reelql) | 视频链接 → 一份 typed JSON：章节/人物/品牌/情感弧线/逐字稿 | 28 | MIT | — |
| ④ | [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI 导演技能：剪辑理论 + Seedance/Kling/Veo 提示词语法 | 455 | CC-BY-4.0 | — |
| ④ | [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | 跨 6 个视频模型端到端出片 + 自我改进质控环 | 6 | MIT | — |
| ④ | [scenario-labs/skills](https://github.com/scenario-labs/skills) | Scenario MCP：按需选模型出图/视频/音频/3D + 驱动 Blender/Maya/Unreal | 751 | MIT | — |
| ④ | [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | 七家供应商智能路由：OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D | 2 | Apache-2.0 | — |
| ④ | [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | 11 个 skill：AI 短剧全流程（剧本 → 分镜 → 提示词 → 成片） | 2,395 | MIT | — |

> 「5.5?」判定口径（逐仓复核各仓库 README 与描述）：**✅** = 明确点名 Opus 5.5；**—** = 未明确点名（多为通用 Claude 技能，通用即兼容 5.5）。**⚠️** = 页面未见标准许可证标识，收录前待确认。**⭐** = 2026-09-30 抓取的 star 快照，仅供粗筛质量参考。

## 分类明细（点标题展开）

### ① 用代码出片 —— 最贴近 Opus 5.5 的工作流

<details>
<summary><b>展开 23 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
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

> makevoid 条目的部分音频/素材走 FAL 生成，需自备 API key（约 $30 + 3M tokens / 3 分钟歌）；其余条目本地代码渲染即可。

</details>

### ② 产品片 / 成片编辑

<details>
<summary><b>展开 7 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
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

### ③ 看视频 / 把视频变成 skill（相邻方向）

<details>
<summary><b>展开 4 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | Teaches your AI to watch videos — learn, absorb, imitate, or give visual feedback。<br>教 AI「看」视频：学习、吸收、复刻，或像真人一样给视觉反馈。 | 多模态视觉 + ffmpeg 抽帧 | `npx skills add Newuxtreme/watch-video-skill` | MIT | — |
| [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | Turns videos and courses into evidence-grounded Agent Skills。<br>把视频和课程转成有据可查的 Agent Skill。 | ffmpeg 抽帧 / 转写 | `npx skills add Lum1104/video-to-skill` | MIT | — |
| [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | Lets Claude watch & understand local videos via ffmpeg + local Whisper; offline, drops into `~/.claude/skills/`。<br>用 ffmpeg + 本地 Whisper 让 Claude 看懂本地视频，离线可用。 | ffmpeg + 本地 Whisper | `npx skills add Moh4696/claude-video-vision` | ⚠️ 未标注* | — |
| [tomascupr/reelql](https://github.com/tomascupr/reelql) | Any video link → one typed JSON: summary / chapters / people / brands / emotion arc / transcript。<br>任意视频链接 → 一份 typed JSON：摘要/章节/人物/品牌/情感弧线/逐字稿。 | 视频理解 API + skill | 见原仓库 README（.claude-plugin） | MIT | — |

</details>

### ④ 调用外部视频模型（非 code-to-video，特意单列）

<details>
<summary><b>展开 5 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills — Murch-style dramaturgy, blocking, montage + exact prompt syntax for Seedance 2.5 / Kling 3.0 / Veo 3.1。<br>AI 导演技能：Murch 剪辑理论、走位、蒙太奇 + Seedance 2.5 / Kling 3.0 / Veo 3.1 精确提示词语法。 | 外部视频模型 API（提示词语法库） | `npx skills add smixs/visual-skills` | CC-BY-4.0 | — |
| [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 models (Seedance 2.0, Kling, Wan, Veo, OmniHuman) with a self-improving QC loop。<br>跨 6 个模型端到端出片，带自我改进的质量控制环。 | 外部视频模型 API + ffmpeg 后期 | `npx skills add 0xadvait/ai-video-skill` | MIT | — |
| [scenario-labs/skills](https://github.com/scenario-labs/skills) | Scenario MCP: smart model picking for image/video/audio/3D + expert skill teams that drive Blender/Maya/Unreal。<br>Scenario MCP：智能选模型出图/视频/音频/3D + 驱动 Blender/Maya/Unreal 的专家 skill 团队。 | Scenario MCP + DCC 软件 | 见原仓库 README | MIT | — |
| [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Smart routing across 7 providers (OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D) with cost gating。<br>七家供应商智能路由（OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D），成本门控。 | 外部模型 API | 见原仓库 README | Apache-2.0 | — |
| [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | 11 skills: full AI short-drama pipeline (source analysis → episodic scripts → storyboard → prompts → film → review)。<br>11 个 skill：AI 短剧/漫剧全流程（原著分析 → 分集剧本 → 分镜 → 提示词 → 成片 → 审查）。 | 视频生成模型 + 剪辑 | 见原仓库 README | MIT | — |

> ④ 类靠托管模型生成像素，与 code-to-video 是两种范式，单列避免混淆。

</details>

## 怎么安装一个 skill

大多数仓库遵循通用 skills 命令行约定：

```bash
npx skills add <owner>/<repo>
```

其他方式：

- 把 skill 目录拷进 `~/.claude/skills/`
- plugin 形态：Claude Code 里 `/plugin marketplace add <owner>/<repo>`，再 `/plugin install <name>`
- 原仓库如果写了自己的安装命令，以原仓库为准

## 相关列表

- [athemeroy/awesome-opus-5-5-videos](https://github.com/athemeroy/awesome-opus-5-5-videos) —— 1000+ 条 Opus 5.5 成片的溯源指南（想直接看片去这里）
- [opusvideo/awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) —— Opus 5.5 视频与动画合集：demo、提示词、工作流（英文 / 中文）
- [LeaddeOpenLab/awesome-opus-5-5-video-prompts](https://github.com/LeaddeOpenLab/awesome-opus-5-5-video-prompts) —— Opus 5.5 视频提示词合集（想直接抄提示词去这里）
- [jacobbubu/claude-opus-5-5-js-animation-research](https://github.com/jacobbubu/claude-opus-5-5-js-animation-research) —— 30 个验证过的 Opus 5.5 浏览器动画案例，按 X 播放量排行（想深挖实现细节去这里）

前两个主要收**成片和工作流**，后两个是**提示词合集与技术案例**；这里收**可安装的 skill**，分工不同。

## 贡献

欢迎 PR —— 先读 [CONTRIBUTING.md](CONTRIBUTING.md)。一句话版本：公开仓库、有可安装的 skill（`SKILL.md` 或 plugin）、能产出或处理视频、标明许可证、**只放链接不拷源码**；新增条目需同时更新 `README.md` 与 `README.en.md` 两份表格。

## 许可与免责声明

- 本索引采用 [MIT](LICENSE) 许可，仓库内不含任何第三方代码，只有链接和简短说明。
- 与 Anthropic 无关联、非官方。Claude 与 Opus 是 Anthropic PBC 的商标。
- 各条目项目保留自己的许可证，一切以原仓库为准。
