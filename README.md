# awesome-opus-video-skills

English: [README.en.md](README.en.md)

一份只收 **开源、可安装的视频类 Agent Skill** 的精选索引——主打 Claude Opus 5.5 真正擅长的出片方式。

**这个列表只讲一件事：** Opus 5.5 出片不是自己画像素，而是**写渲染代码**——Canvas、Remotion、p5.js、GSAP——用无头浏览器逐帧渲染，再用 ffmpeg 合成。这里收的 skill 就是把这条流水线打包好，装上就能说：「给我做一条 60 秒的 XX 视频」。

本仓库只放**链接**，不托管任何第三方源码。每条固定字段：一句话用途、渲染栈、安装命令、许可证、是否专为 Opus 5.5。

## ⚡ 速览全部 17 个 skill

分类：**①** 用代码出片 · **②** 产品片/成片编辑 · **③** 看视频/视频转 skill · **④** 调用外部视频模型

| # | Skill | 一句话用途 | License | 5.5? |
| --- | --- | --- | --- | --- |
| ① | [klsoen/opus-js-animations](https://github.com/klsoen/opus-js-animations) | 导演式出片：brief → 配音 → 导演阐述 → JS 渲染帧级精确 MP4 | MIT | ✅ |
| ① | [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | Remotion 电影感产品宣传片：152 张镜头配方卡 + 生产级模板 | Apache-2.0 | — |
| ① | [bestagentkits/motion-video-skill](https://github.com/bestagentkits/motion-video-skill) | HyperFrames + GSAP 节拍同步 1080p：AI 配音、卡拉 OK 字幕 | MIT | — |
| ① | [haidrrrry/claude-remotion-skill](https://github.com/haidrrrry/claude-remotion-skill) | 教 Claude 用 Remotion 做动态图形：剪辑、B-roll、字幕、配乐 | MIT | — |
| ① | [JohnHeibel/ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | 手绘动画底板：p5.js + Clawd 角色 + 31 种表演情绪 | MIT | ✅ |
| ① | [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) | 给成片加运动图形 B-roll（Claude Code / Codex） | ⚠️ 未标注 | — |
| ① | [Changroro/code-video](https://github.com/Changroro/code-video) | 调研主题后渲染手绘 + 8-bit 宣传短片 | MIT | ✅ |
| ① | [JagZ999/explainer-video](https://github.com/JagZ999/explainer-video) | 产品讲解动画：配音、音乐、同步音效 | MIT | — |
| ① | [misbahsy/claude-horizon-animation](https://github.com/misbahsy/claude-horizon-animation) | 复刻 Opus 5.5 发布公告风格动画 | ⚠️ 未标注 | ✅ |
| ② | [browser-use/video-use](https://github.com/browser-use/video-use) | 用编码 Agent 剪成片：精剪、字幕、调色、叠加动画 | MIT | — |
| ② | [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | 运动设计基础（节奏/字体/色彩/构图）+ Remotion 引擎 | MIT | — |
| ② | [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram / intro / outro 频道包装件 | MIT | — |
| ③ | [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | 教 AI「看」视频：学习、吸收、复刻、视觉反馈 | MIT | — |
| ③ | [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | 把视频和课程转成有据可查的 Agent Skill | MIT | — |
| ③ | [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | ffmpeg + 本地 Whisper 看懂本地视频（离线可用） | ⚠️ 未标注 | — |
| ④ | [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI 导演技能：剪辑理论 + Seedance/Kling/Veo 提示词语法 | CC-BY-4.0 | — |
| ④ | [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | 跨 6 个视频模型端到端出片 + 自我改进质控环 | MIT | — |

> 「5.5?」判定口径（2026-09-27 逐仓复核各仓库 README 与描述）：**✅** = 明确点名 Opus 5.5；**—** = 未明确点名（多为通用 Claude 技能，通用即兼容 5.5）。**⚠️** = 页面未见标准许可证标识，收录前待确认。

## 分类明细（点标题展开）

### ① 用代码出片 —— 最贴近 Opus 5.5 的工作流

<details>
<summary><b>展开 9 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [klsoen/opus-js-animations](https://github.com/klsoen/opus-js-animations) | Director-style flow: brief → voiceover → treatment → frame-exact MP4, rendered in JavaScript。<br>导演式出片：brief → 配音 → 导演阐述 → JS 渲染帧级精确 MP4。 | JS + Chrome 逐帧渲染 + ffmpeg，AI 配音 | `npx skills add klsoen/opus-js-animations` | MIT | **Yes** |
| [Vincentwei1021/video-shotcraft](https://github.com/Vincentwei1021/video-shotcraft) | Cinematic product promos in Remotion: 152 shot recipe cards, 209 motion previews, production-ready template。<br>Remotion 电影感产品宣传片：152 张镜头配方卡、209 个动效预览、生产级模板。 | Remotion | `npx skills add Vincentwei1021/video-shotcraft` | Apache-2.0 | — |
| [bestagentkits/motion-video-skill](https://github.com/bestagentkits/motion-video-skill) | Beat-synced 1080p motion graphics in HyperFrames (HTML + GSAP) with AI voice-over, karaoke captions, SFX & generated music。<br>HyperFrames + GSAP 出节拍同步 1080p 动态视频：AI 配音、卡拉 OK 字幕、音效与生成音乐。 | HyperFrames（HTML + GSAP）+ ffmpeg | `npx skills add bestagentkits/motion-video-skill` | MIT | — |
| [haidrrrry/claude-remotion-skill](https://github.com/haidrrrry/claude-remotion-skill) | Teaches Claude to build professional motion-graphics videos with Remotion: editing, B-roll, captions, sound。<br>教 Claude 用 Remotion 做专业动态图形：剪辑、B-roll、字幕、配乐。 | Remotion + ffmpeg | 见原仓库 README（skill 在子目录） | MIT | — |
| [JohnHeibel/ClaudeAnimationBase](https://github.com/JohnHeibel/ClaudeAnimationBase) | Starter kit for hand-painted cartoons: p5.js + p5.brush, the Clawd character, 31 acted emotions。<br>手绘动画底板：p5.js + p5.brush、Clawd 角色、31 种表演情绪。 | p5.js（p5.brush）+ Playwright + ffmpeg | 见原仓库 README | MIT | **Yes** |
| [Barty-Bart/motion-graphics](https://github.com/Barty-Bart/motion-graphics) | Motion-graphics skill pack for Claude Code / Codex — adds MG B-roll to your footage。<br>Claude Code / Codex 运动图形技能包：给成片加 MG B-roll。 | Playwright + ffmpeg | 见原仓库 README（多 skill 子目录） | ⚠️ 未标注* | — |
| [Changroro/code-video](https://github.com/Changroro/code-video) | Researches a topic, then renders a hand-drawn + 8-bit promo video (MP4)。<br>调研主题后渲染手绘 + 8-bit 风格宣传短片（MP4）。 | 代码逐帧绘制 + ffmpeg | `npx skills add Changroro/code-video` | MIT | **Yes** |
| [JagZ999/explainer-video](https://github.com/JagZ999/explainer-video) | Animated product explainer videos with voiceover, music & synced SFX。<br>带配音、音乐与同步音效的产品讲解动画。 | Puppeteer 渲染 + ffmpeg + ElevenLabs | `npx skills add JagZ999/explainer-video` | MIT | — |
| [misbahsy/claude-horizon-animation](https://github.com/misbahsy/claude-horizon-animation) | Recreates the Claude Opus 5.5 announcement-style animation。<br>复刻 Claude Opus 5.5 发布公告风格的动画。 | 浏览器逐帧渲染 + ffmpeg | `npx skills add misbahsy/claude-horizon-animation` | ⚠️ 未标注* | **Yes** |

\* 页面未显示标准许可证标识，可能是自定义许可证；收录前需到原仓库确认。Page shows no standard SPDX license badge — confirm in the source repo.

</details>

### ② 产品片 / 成片编辑

<details>
<summary><b>展开 3 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [browser-use/video-use](https://github.com/browser-use/video-use) | Edit videos with coding agents — structural cuts, captions, color, overlaid animation。<br>用编码 Agent 剪成片：结构精剪、字幕、调色、叠加动画。 | ffmpeg + Remotion / HyperFrames 叠加 + TTS | `npx skills add browser-use/video-use` | MIT | — |
| [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | Motion-design fundamentals (timing, typography, color, composition) + Remotion engine as installable skills。<br>运动设计基础（节奏、字体、色彩、构图）+ Remotion 引擎，做成可安装技能。 | Remotion | `npx skills add iart-ai/motion-design-skills` | MIT | — |
| [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram + YouTube intro/outro skills — turn every episode into channel branding。<br>Audiogram / YouTube intro / outro：把每期节目变成频道包装件。 | 模板化运动图形 + 旁白 | `npx skills add iart-ai/youtube-video-skills` | MIT | — |

</details>

### ③ 看视频 / 把视频变成 skill（相邻方向）

<details>
<summary><b>展开 3 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | Teaches your AI to watch videos — learn, absorb, imitate, or give visual feedback。<br>教 AI「看」视频：学习、吸收、复刻，或像真人一样给视觉反馈。 | 多模态视觉 + ffmpeg 抽帧 | `npx skills add Newuxtreme/watch-video-skill` | MIT | — |
| [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | Turns videos and courses into evidence-grounded Agent Skills。<br>把视频和课程转成有据可查的 Agent Skill。 | ffmpeg 抽帧 / 转写 | `npx skills add Lum1104/video-to-skill` | MIT | — |
| [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | Lets Claude watch & understand local videos via ffmpeg + local Whisper; offline, drops into `~/.claude/skills/`。<br>用 ffmpeg + 本地 Whisper 让 Claude 看懂本地视频，离线可用。 | ffmpeg + 本地 Whisper | `npx skills add Moh4696/claude-video-vision` | ⚠️ 未标注* | — |

</details>

### ④ 调用外部视频模型（非 code-to-video，特意单列）

<details>
<summary><b>展开 2 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills — Murch-style dramaturgy, blocking, montage + exact prompt syntax for Seedance 2.5 / Kling 3.0 / Veo 3.1。<br>AI 导演技能：Murch 剪辑理论、走位、蒙太奇 + Seedance 2.5 / Kling 3.0 / Veo 3.1 精确提示词语法。 | 外部视频模型 API（提示词语法库） | `npx skills add smixs/visual-skills` | CC-BY-4.0 | — |
| [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 models (Seedance 2.0, Kling, Wan, Veo, OmniHuman) with a self-improving QC loop。<br>跨 6 个模型端到端出片，带自我改进的质量控制环。 | 外部视频模型 API + ffmpeg 后期 | `npx skills add 0xadvait/ai-video-skill` | MIT | — |

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

它们主要收**成片和工作流**，这里收**可安装的 skill**，重合度低、分工不同。

## 贡献

欢迎 PR —— 先读 [CONTRIBUTING.md](CONTRIBUTING.md)。一句话版本：公开仓库、有可安装的 skill（`SKILL.md` 或 plugin）、能产出或处理视频、标明许可证、**只放链接不拷源码**；新增条目需同时更新 `README.md` 与 `README.en.md` 两份表格。

## 许可与免责声明

- 本索引采用 [MIT](LICENSE) 许可，仓库内不含任何第三方代码，只有链接和简短说明。
- 与 Anthropic 无关联、非官方。Claude 与 Opus 是 Anthropic PBC 的商标。
- 各条目项目保留自己的许可证，一切以原仓库为准。
