# awesome-opus-video-skills

一份只收 **开源、可安装的视频类 Agent Skill** 的精选索引——主打 Claude Opus 5.5 真正擅长的出片方式。English: [README.md](README.md)

**这个列表只讲一件事：** Opus 5.5 出片不是自己画像素，而是**写渲染代码**——Canvas、Remotion、p5.js、GSAP——用无头浏览器逐帧渲染，再用 ffmpeg 合成。这里收的 skill 就是把这条流水线打包好，装上就能说：「给我做一条 60 秒的 XX 视频」。

本仓库只放**链接**，不托管任何第三方源码。每条固定字段：一句话用途、渲染栈、安装命令、许可证、是否专为 Opus 5.5。

→ 完整列表见 **[skills.md](skills.md)**（中英双语条目）

## 分类

1. **用代码出片** —— 最贴近 Opus 5.5 的工作流：模型写渲染代码，浏览器逐帧出图，ffmpeg 合成 MP4。确定性渲染、可复现、没有生成式闪烁。
2. **产品片 / 成片编辑** —— 处理已有素材：结构精剪、字幕、调色、运动图形叠加、片头片尾。
3. **看视频 / 视频转 skill**（相邻方向）—— 不是做视频，而是让 Agent **看懂**视频，或把视频沉淀成可复用技能。
4. **调用外部视频模型**（特意单列）—— 调 Seedance / Kling / Veo 这类托管 API 出片。有用，但和 code-to-video 是两种范式。

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

- [athemeroy/awesome-opus-5-5-videos](https://github.com/athemeroy/awesome-opus-5-5-videos) —— 1000+ 条 Opus 5.5 成片的溯源指南
- [opusvideo/awesome-claude-video](https://github.com/opusvideo/awesome-claude-video) —— Opus 5.5 视频与动画合集：demo、提示词、工作流（英文 / 中文）

它们主要收**成片和工作流**，这里收**可安装的 skill**——重合度低，分工不同。

## 贡献

欢迎 PR —— 先读 [CONTRIBUTING.md](CONTRIBUTING.md)。一句话版本：公开仓库、有可安装的 skill（`SKILL.md` 或 plugin）、能产出或处理视频、标明许可证、**只放链接不拷源码**。

## 许可与免责声明

- 本索引采用 [MIT](LICENSE) 许可，仓库内不含任何第三方代码，只有链接和简短说明。
- 与 Anthropic 无关联、非官方。Claude 与 Opus 是 Anthropic PBC 的商标。
- 各条目项目保留自己的许可证，一切以原仓库为准。
