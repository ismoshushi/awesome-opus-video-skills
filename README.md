# awesome-opus-video-skills

English: [README.en.md](README.en.md)

一份只收 **开源、可安装的视频类 Agent Skill** 的精选索引——主打 Claude Opus 5.5 真正擅长的出片方式。

**这个列表只讲一件事：** Opus 5.5 出片不是自己画像素，而是**写渲染代码**——Canvas、Remotion、p5.js、GSAP——用无头浏览器逐帧渲染，再用 ffmpeg 合成。这里收的 skill 就是把这条流水线打包好，装上就能说：「给我做一条 60 秒的 XX 视频」。

本仓库只放**链接**，不托管任何第三方源码。每条固定字段：一句话用途、渲染栈、安装命令、许可证、是否专为 Opus 5.5。

## ⚡ 速览全部 40 个 skill

分类：**①** 用代码出片 · **②** 产品片/成片编辑 · **③** 看视频/视频转 skill · **④** 调用外部视频模型

| # | Skill | 一句话用途 | License | 5.5? |
| --- | --- | --- | --- | --- |
| ① | [klsoen/opus-js-animations](https://github.com/klsoen/opus-js-animations) | 导演式出片：brief → 配音 → 导演阐述 → JS 渲染帧级精确 MP4 | MIT | ✅ |
| ① | [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | Remotion 电影感产品宣传片：152 张镜头配方卡 + 生产级模板 | Apache-2.0 | — |
| ① | [bestagentkits/motion-video-skill](https://github.com/bestagentkits/motion-video-skill) | HyperFrames + GSAP 节拍同步 1080p：AI 配音、卡拉 OK 字幕 | MIT | — |
| ① | [haidrrrry/claude-remotion-skill](https://github.com/haidrrrry/claude-remotion-skill) | 教 Claude 用 Remotion 做动态图形：剪辑、B-roll、字幕、配乐 | MIT | — |
| ① | [JohnHeibel/ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | 手绘动画底板：p5.js + Clawd 角色 + 31 种表演情绪 | MIT | ✅ |
| ① | [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) | 给成片加运动图形 B-roll（Claude Code / Codex） | MIT | — |
| ① | [Changroro/code-video](https://github.com/Changroro/code-video) | 调研主题后渲染手绘 + 8-bit 宣传短片 | MIT | ✅ |
| ① | [JagZ999/explainer-video](https://github.com/JagZ999/explainer-video) | 产品讲解动画：配音、音乐、同步音效 | MIT | — |
| ① | [misbahsy/claude-horizon-animation](https://github.com/misbahsy/claude-horizon-animation) | 复刻 Opus 5.5 发布公告风格动画 | ⚠️ 未标注 | ✅ |
| ① | [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | 专为 Opus 5.5 打造：逐帧逐音符全代码生成，一种风格一个 skill | MIT | ✅ |
| ① | [howseen-ai/claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | 纯代码运动设计视频：HTML + Playwright + ffmpeg，无需 AE/Remotion | MIT | ✅ |
| ① | [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | 一段音乐 + 一句提示词 → 高品质 MG 视频（Opus 5.5 plugin） | MIT | ✅ |
| ① | [echris6/motion-video-kit](https://github.com/echris6/motion-video-kit) | 商业级视频包：独立评审环 + 28 部 launch film 运动原则 | MIT | — |
| ① | [Kimeur/motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) | brief → 循环动态字体 launch 视频（单文件 HTML 确定性渲染） | MIT | — |
| ① | [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple 风格发布片：代码逐帧渲染 + 卡点配乐配音 | MIT | ✅ |
| ① | [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | 确定性 seek(t) + 自动渲染质检，纯文本模型也能出 MP4 | MIT | — |
| ① | [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | 代码渲染 MG 影片：标注预览 + 卡点授权音乐 + 盲听质检 | MIT | — |
| ① | [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | 自主 Code-to-Video 引擎：HyperFrames + GSAP + Whisper + TTS | MIT | ✅ |
| ① | [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | DIY 纸拼贴风视频（HyperFrames） | MIT | — |
| ① | [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | showreel 级代码 MG，每条配原创配乐 | MIT | — |
| ① | [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | 旁白 + 真实素材 + 任选画风 → 短片 | MIT | ✅ |
| ① | [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | 可编辑 HTML/JS 场景 + 口播版式，本地导出校验 MP4 | MIT | — |
| ① | [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | 主题/脚本 → 旁白 MP4：HTML 幻灯 + TTS + ASR 校验 | MIT | — |
| ① | [FavioVazquez/showtime](https://github.com/FavioVazquez/showtime) | 面向编码 Agent 的本地视频工作室：一句话生成动态图形、配音、配乐与字幕，全程本机渲染 | MIT | — |
| ② | [browser-use/video-use](https://github.com/browser-use/video-use) | 用编码 Agent 剪成片：精剪、字幕、调色、叠加动画 | MIT | — |
| ② | [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | 运动设计基础（节奏/字体/色彩/构图）+ Remotion 引擎 | MIT | — |
| ② | [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram / intro / outro 频道包装件 | MIT | — |
| ② | [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | 对话式视频编辑器：多轨时间线 + MCP + Remotion 渲染 | AGPL-3.0 | — |
| ② | [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | 真人口播全屏舞台视觉包装（Remotion + 审核帧验证） | MIT | — |
| ② | [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | 口播剪辑包装引擎：分镜驱动 MG + 可复用镜头库 | Apache-2.0 | — |
| ② | [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | 语音便签 → 带动画音效的短视频 | MIT | — |
| ③ | [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | 教 AI「看」视频：学习、吸收、复刻、视觉反馈 | MIT | — |
| ③ | [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | 把视频和课程转成有据可查的 Agent Skill | MIT | — |
| ③ | [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | ffmpeg + 本地 Whisper 看懂本地视频（离线可用） | ⚠️ 未标注 | — |
| ③ | [tomascupr/reelql](https://github.com/tomascupr/reelql) | 视频链接进、结构化 JSON 出，给 Agent 装眼睛 | MIT | — |
| ④ | [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI 导演技能：剪辑理论 + Seedance/Kling/Veo 提示词语法 | CC-BY-4.0 | — |
| ④ | [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | 跨 6 个视频模型端到端出片 + 自我改进质控环 | MIT | — |
| ④ | [scenario-labs/skills](https://github.com/scenario-labs/skills) | 图/视频/音频/3D 生成：自动选模型 + 先报价再花 | MIT | — |
| ④ | [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | 通用视觉生成：多家模型 + 智能成本闸门 | Apache-2.0 | — |
| ④ | [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | AI 短剧/漫剧创作全家桶：剧本→分镜→提示词 | MIT | — |

> 「5.5?」判定口径（首批 2026-09-27、新增批次 2026-09-29 逐仓复核各仓库 README 与描述）：**✅** = 明确点名 Opus 5.5；**—** = 未明确点名（多为通用 Claude 技能，通用即兼容 5.5）。**⚠️** = 页面未见标准许可证标识，收录前待确认。

## 分类明细（点标题展开）

### ① 用代码出片 —— 最贴近 Opus 5.5 的工作流

<details>
<summary><b>展开 24 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
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
| [FavioVazquez/showtime](https://github.com/FavioVazquez/showtime) | Local video studio for coding agents: one sentence in, a finished MP4 (and a single-file HTML video) out, with motion graphics, local voice-over, a 249-track music catalog with automatic credits, captions and QA checks; works in Claude Code, Codex, Cursor, Devin and OpenCode。<br>面向编码 Agent 的本地视频工作室：一句话生成成片（MP4 与单文件 HTML 视频），含动态图形、本地配音、249 首带自动署名的配乐、字幕与质检；支持 Claude Code、Codex、Cursor、Devin、OpenCode。 | Headless Chrome + ffmpeg + local TTS | `npx skills add FavioVazquez/showtime` | MIT | — |

\* 页面未显示标准许可证标识，可能是自定义许可证；收录前需到原仓库确认。Page shows no standard SPDX license badge — confirm in the source repo.

> makevoid 条目的部分音频/素材走 FAL 生成，需自备 API key（一条视频约 $30）；其余条目本地代码渲染即可。

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
| [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | Open-source, local-first conversational AI video editor: professional multi-track timeline, Agent Skills, MCP integration, Remotion rendering。<br>开源、本地优先的对话式视频编辑器：专业多轨时间线 + Agent Skills + MCP + Remotion 渲染。 | 多轨时间线 + Remotion 渲染 | 见原仓库 README（应用形态，内嵌 skill） | AGPL-3.0 | — |
| [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | Talking-head full-screen stage visual packaging: Remotion compositing, plan approval, review frames and final-output verification。<br>真人口播全屏舞台视觉包装 Skill：Remotion 合成、方案审批、审核帧与成片验证。 | Remotion 合成 + 审批/审核帧流程 | `npx skills add cytxnyu/chuanyuntian-auto-edit-pro` | MIT | — |
| [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | Talking-head editing & packaging engine: storyboard-driven motion graphics, reusable shot library, director skill (Claude Code / Codex)。<br>口播视频剪辑与包装引擎：分镜驱动运动图形 + 可复用镜头库 + 导演 Skill。 | 分镜驱动 MG + 镜头库 | `npx skills add xiaolu-ai26/xiaolu-motion` | Apache-2.0 | — |
| [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | Turn a voice note into an animated, sound-designed Short。<br>一条语音便签 → 带动画与音效设计的竖屏短视频。 | 代码动画 + 音效设计 | `npx skills add Dancan254/voiceover-video-skill` | MIT | — |

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
| [tomascupr/reelql](https://github.com/tomascupr/reelql) | Give your agent eyes: any video link in, one typed JSON out. A Claude skill + API。<br>给 Agent 装上眼睛：任意视频链接进，一个结构化 JSON 出（skill + API）。 | 视频理解 API（结构化输出） | `/plugin marketplace add tomascupr/reelql` | MIT | — |

</details>

### ④ 调用外部视频模型（非 code-to-video，特意单列）

<details>
<summary><b>展开 5 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills — Murch-style dramaturgy, blocking, montage + exact prompt syntax for Seedance 2.5 / Kling 3.0 / Veo 3.1。<br>AI 导演技能：Murch 剪辑理论、走位、蒙太奇 + Seedance 2.5 / Kling 3.0 / Veo 3.1 精确提示词语法。 | 外部视频模型 API（提示词语法库） | `npx skills add smixs/visual-skills` | CC-BY-4.0 | — |
| [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 models (Seedance 2.0, Kling, Wan, Veo, OmniHuman) with a self-improving QC loop。<br>跨 6 个模型端到端出片，带自我改进的质量控制环。 | 外部视频模型 API + ffmpeg 后期 | `npx skills add 0xadvait/ai-video-skill` | MIT | — |
| [scenario-labs/skills](https://github.com/scenario-labs/skills) | Production-ready images, video, audio and 3D from any AI agent: picks the right model, prices before spending, keeps characters & brands consistent (Scenario MCP)。<br>生产级图/视频/音频/3D 生成：自动选模型、先报价再花、角色与品牌一致性（Scenario MCP）。 | Scenario MCP + 托管模型 API | `npx skills add scenario-labs/skills` | MIT | — |
| [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Universal visual generation skill — images, SVG, video, audio via OpenAI, Gemini, FAL, KIE, HeyGen, ElevenLabs with smart cost gating。<br>通用视觉生成 skill：图/SVG/视频/音频走多家模型，带智能成本闸门。 | OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs API | `npx skills add hectorcanaimero/da-vinci` | Apache-2.0 | — |
| [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | Open-source AI short-drama skills for Claude Code & Codex: script, character assets, storyboard, image/video prompts, review。<br>开源 AI 短剧/漫剧创作 skill 合集：剧本、角色资产、分镜、图/视频提示词、审查。 | 剧本 → 分镜 → 图/视频提示词流水线 | `npx skills add zenstory-ai/drama-skills` | MIT | — |

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
- [jacobbubu/claude-opus-5-5-js-animation-research](https://github.com/jacobbubu/claude-opus-5-5-js-animation-research) —— Opus 5.5 JS 动画技术研究笔记（想深挖实现细节去这里）

前两个主要收**成片和工作流**，后两个是**提示词合集与技术笔记**；这里收**可安装的 skill**，分工不同。

## 贡献

欢迎 PR —— 先读 [CONTRIBUTING.md](CONTRIBUTING.md)。一句话版本：公开仓库、有可安装的 skill（`SKILL.md` 或 plugin）、能产出或处理视频、标明许可证、**只放链接不拷源码**；新增条目需同时更新 `README.md` 与 `README.en.md` 两份表格。

## 许可与免责声明

- 本索引采用 [MIT](LICENSE) 许可，仓库内不含任何第三方代码，只有链接和简短说明。
- 与 Anthropic 无关联、非官方。Claude 与 Opus 是 Anthropic PBC 的商标。
- 各条目项目保留自己的许可证，一切以原仓库为准。
