# awesome-opus-video-skills

English: [README.en.md](README.en.md)

一份只收 **开源、可安装的视频类 Agent Skill** 的精选索引——主打 Claude Opus 5.5 真正擅长的出片方式。

**这个列表只讲一件事：** Opus 5.5 出片不是自己画像素，而是**写渲染代码**——Canvas、Remotion、p5.js、GSAP——用无头浏览器逐帧渲染，再用 ffmpeg 合成。这里收的 skill 就是把这条流水线打包好，装上就能说：「给我做一条 60 秒的 XX 视频」。

本仓库只放**链接**，不托管任何第三方源码。每条固定字段：一句话用途、渲染栈、安装命令、许可证、是否专为 Opus 5.5。

## ⚡ 速览全部 118 个 skill

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
| ① | [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple 风产品发布片：__seek(t) + headless Chrome + ElevenLabs | 1 | MIT | — |
| ① | [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | 纪律化 motion pipeline：自动 QA + 自创配乐 | 1 | MIT | — |
| ① | [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | 代码短片 + 可标注实时预览 + 盲读质检 | 0 | MIT | — |
| ① | [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | HyperFrames + GSAP + Whisper 词级对齐的 6 步出片管线 | 3 | MIT | ✅ |
| ① | [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | 纸拼贴风竖屏视频：HyperFrames 模板化出片 | 3 | MIT | — |
| ① | [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | 从链接读品牌 → 出片 + 自研合成器原创配乐 | 13 | MIT | — |
| ① | [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | 自己的旁白 + 真实素材 → 6 种风格 20–60 秒 promo | 12 | MIT | ✅ |
| ① | [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | 真人口播编排：HTML/JS 动效 + Chromium 逐帧 + ffmpeg | 18 | MIT | — |
| ① | [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | HTML 幻灯片 + TTS + ASR 回译校验 → 口播 MP4（中/英/粤） | 1 | MIT | — |
| ① | [unclejobs-ai/motion-video-skill](https://github.com/unclejobs-ai/motion-video-skill) | 韩文 motion graphics skill：出片顺序 + 分阶段检查 harness | 102 | MIT | — |
| ① | [Tejashmakwana/motionmaxxing](https://github.com/Tejashmakwana/motionmaxxing) | 「给动态图形整容」：把 AI 味重的视频修成像人做的片子 | 76 | Apache-2.0 | — |
| ① | [EGSECDA/vocaloid-style-mv-pipeline](https://github.com/EGSECDA/vocaloid-style-mv-pipeline) | Vocaloid 风手绘歌词 MV 生产管线 + Claude Code skill（三语文档） | 51 | MIT | — |
| ① | [minosdevs/cinematic-film](https://github.com/minosdevs/cinematic-film) | 任意主题 → Remotion + three.js 电影感动画短片 | 21 | MIT | — |
| ① | [ouerf-man/product-launch-motion-skill](https://github.com/ouerf-man/product-launch-motion-skill) | 纯代码产品/功能发布片：HyperFrames + GSAP | 15 | MIT | — |
| ① | [direkturcrypto/remotion-opus-skill](https://github.com/direkturcrypto/remotion-opus-skill) | Remotion Opus skill（附带 cli/bin） | 11 | MIT | — |
| ① | [Neelshah1810/Claude-Video-Skills](https://github.com/Neelshah1810/Claude-Video-Skills) | 11 个 skill：launch films、explainers、social ads、testimonial 等 | 7 | MIT | — |
| ① | [seoddhh/apple-style-promo-video-skills](https://github.com/seoddhh/apple-style-promo-video-skills) | Apple 风 promo 视频 skills | 7 | MIT | — |
| ① | [Win-Hao/knowledge-video](https://github.com/Win-Hao/knowledge-video) | 一个主题 → 1–3 分钟知识讲解视频（fact-checked） | 6 | MIT | — |
| ① | [Win-Hao/code-video](https://github.com/Win-Hao/code-video) | 用代码做短视频：agent 先问需求，再写 seven-block prompt | 6 | MIT | — |
| ① | [farming-labs/product-film-skill](https://github.com/farming-labs/product-film-skill) | 产品发布片 = 单个 HTML 文件，导出 MP4 | 6 | MIT | — |
| ① | [mos-ski/motion-video-skill](https://github.com/mos-ski/motion-video-skill) | Figma/产品 URL → Remotion 动态图形成片：节拍分镜 + 自评打分 8+ | 8 | MIT | — |
| ① | [cpp285/gold-noir-video-creator](https://github.com/cpp285/gold-noir-video-creator) | 暗金风科普视频：Remotion + Three.js、逐字字幕、程序配乐（中文） | 3 | MIT | — |
| ① | [makevoid/motion-graphics-music-video-skill-noimage](https://github.com/makevoid/motion-graphics-music-video-skill-noimage) | makevoid 原版的 noimage 变体：纯代码，不调用图像模型 | 2 | MIT | ✅ |
| ① | [RohanRatwani/explainer-video-opus-5.5](https://github.com/RohanRatwani/explainer-video-opus-5.5) | 主题 → motion-design 讲解视频（16:9 或 Shorts） | — | MIT | ✅ |
| ① | [Everett406/code-film](https://github.com/Everett406/code-film) | Director-level 代码视频（Remotion），注明 Built with Opus 5.5 | — | MIT | ✅ |
| ① | [lumian2015/opus-5-5-video-templates](https://github.com/lumian2015/opus-5-5-video-templates) | 30 个从 viral Opus 5.5 视频复刻的 MG 模板 + skill | — | MIT | ✅ |
| ① | [ARTHONG1/Opus-promo-Director](https://github.com/ARTHONG1/Opus-promo-Director) | 短节拍同步 promo：look-first 风格帧 + Remotion 自审出片 | — | MIT | — |
| ① | [02ui/02ui-video-copy](https://github.com/02ui/02ui-video-copy) | HyperFrames launch 视频 + motion library + AI 动效检查 | — | MIT | — |
| ① | [dEitY719/video-skills](https://github.com/dEitY719/video-skills) | 参数化 HyperFrames motion-graphic recipes（多 harness） | — | MIT | — |
| ① | [Saucemathis/marketing-video-skill](https://github.com/Saucemathis/marketing-video-skill) | 任意品牌成片营销视频：morphing UI、真实光标 | — | MIT | — |
| ① | [harish-anumula/launch-video-skill](https://github.com/harish-anumula/launch-video-skill) | 代码产品发布片：story shapes + Remotion | — | MIT | — |
| ① | [JudgePeach/remotion-shotflow](https://github.com/JudgePeach/remotion-shotflow) | 参考引导的 Remotion 视频：8 shot recipes | — | MIT | — |
| ① | [GroMarketing/remotion-qa](https://github.com/GroMarketing/remotion-qa) | Remotion 成片 QA：Reels/Shorts 安全区检查 | — | MIT | — |
| ① | [salomonMuriel/media-production-skills](https://github.com/salomonMuriel/media-production-skills) | Director-level 视频（Remotion）+ 脚本 + AI 配音 + 音效 | — | MIT | — |
| ① | [jerelvelarde/demo-skills](https://github.com/jerelvelarde/demo-skills) | Launch video + UI mockup 动画 skills | — | MIT | — |
| ① | [KJ-AIML/product-launch-film](https://github.com/KJ-AIML/product-launch-film) | Agent skill + Remotion starter：代码渲染产品发布片 | — | MIT | — |
| ① | [Anann99/launch-film-skill](https://github.com/Anann99/launch-film-skill) | 网站 + 真实产品 → expert-grade launch film | — | MIT | — |
| ① | [NDilanka/openvids](https://github.com/NDilanka/openvids) | Remotion launch 风产品视频 + 程序配乐 | — | MIT | — |
| ① | [JBJMLLC/demo-studio](https://github.com/JBJMLLC/demo-studio) | Story-first 产品 demos：可组合 skills + 浏览器录制 + 旁白 | — | MIT | — |
| ① | [q2522879285-source/code-music-video-skill](https://github.com/q2522879285-source/code-music-video-skill) | 确定性音乐驱动代码视频：workflow + 时间轴校验 | — | MIT | — |
| ① | [patt-rick/app-promo-motion](https://github.com/patt-rick/app-promo-motion) | 真实 UI 的 motion-graphics app promo（Remotion） | 2 | MIT | — |
| ① | [WizerdBaChe/motion-video-skill](https://github.com/WizerdBaChe/motion-video-skill) | 代码渲染视频（ads/product tours/showreels） | 1 | MIT | — |
| ① | [authrain-cloud-abdullahformuli/explainer-video-skills](https://github.com/authrain-cloud-abdullahformuli/explainer-video-skills) | explainer 视频 skills：脚本/分镜/渲染旁白 | 1 | MIT | — |
| ① | [yuchenmax88-wq/lingcut-video-skill](https://github.com/yuchenmax88-wq/lingcut-video-skill) | AI 影视流水线：LingCut + LibTV + ffmpeg，尾帧接续法（中文） | — | MIT | — |
| ① | [Annie-246/tabcom-skills](https://github.com/Annie-246/tabcom-skills) | carousel、video edit、social QA video skills | — | MIT | — |
| ① | [zeana9658-alt/remotion-particle-film](https://github.com/zeana9658-alt/remotion-particle-film) | 60 秒程序粒子短片 + Codex skill | 1 | MIT | — |
| ① | [huynhcongdac/story-video-skill](https://github.com/huynhcongdac/story-video-skill) | AI agent 讲故事视频 3–5 分钟（越南语） | 1 | MIT | — |
| ① | [124zhe/xigua-msvideo-skill](https://github.com/124zhe/xigua-msvideo-skill) | Codex skills：YouTube 好奇心故事 + MS Paint 分镜 + 旁白组装 | 2 | MIT | — |
| ① | [jttriana86/claude-video-skill](https://github.com/jttriana86/claude-video-skill) | 代码动画视频 + AI 配音词级同步（西语） | — | MIT | — |
| ① | [Kianzzz/xilo-opus-video](https://github.com/Kianzzz/xilo-opus-video) | 通用型：想法/文章/参考视频 → 多套方案预览 → 成片 | 104 | MIT | ✅ |
| ① | [lemomo-ai/lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | 43 种影片风格图册，按风格名生成 | 2,270 | MIT | ✅ |
| ① | [chuspeeism/dashi-animationstyle](https://github.com/chuspeeism/dashi-animationstyle) | 中文口播配画面：15–60 秒，7 套画风，带字幕可导剪映 | 29 | MIT | ✅ |
| ① | [alchaincyf/huashu-art-motion](https://github.com/alchaincyf/huashu-art-motion) | 美术史题材：35 种可动化艺术风格 + 9 种解说讲法 | 3,931 | MIT | — |
| ① | [WaterDJiang/Wattter_openSkills](https://github.com/WaterDJiang/Wattter_openSkills) | 一站式：想法 → 中文剧本 + 分镜 + 可改源码 + 带声音 MP4 | 45 | ⚠️ 未标注 | — |
| ① | [Vincentwei1021/mg-styles-15](https://github.com/Vincentwei1021/mg-styles-15) | 15 种 MG 风格，每支约 10 秒，附提示词 + 源码（非可安装 skill） | 818 | MIT | ✅ |
| ① | [nutllwhy/code-brand-film](https://github.com/nutllwhy/code-brand-film) | 用代码做 15 秒品牌宣传片：单页 HTML + GSAP 时间轴 → HyperFrames 逐帧渲染，配乐 Python 合成原创曲、节拍跟切点 | 14 | MIT | — |
| ① | [imraywang/rayskills](https://github.com/imraywang/rayskills) | ray-explainer：文章/观点 → 知识解说视频（默认竖屏 1.5–3 分钟，配音+字幕），canvas/JS 逐帧代码绘制；仓库共 8 个 skill | 173 | CC BY-NC 4.0（非商业） | — |
| ② | [browser-use/video-use](https://github.com/browser-use/video-use) | 用编码 Agent 剪成片：精剪、字幕、调色、叠加动画 | 27,657 | MIT | — |
| ② | [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | 运动设计基础（节奏/字体/色彩/构图）+ Remotion 引擎 | 39 | MIT | — |
| ② | [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram / intro / outro 频道包装件 | 4 | MIT | — |
| ② | [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | 对话式 AI 剪辑器：Agent Skills + MCP + Remotion，多轨时间线 | 2,056 | AGPL-3.0 | — |
| ② | [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | 口播全屏视觉舞台包装：Remotion + 分阶段审核 | 1 | MIT | — |
| ② | [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | 口播动效底座 + 几十个镜头库：透明层 + ffmpeg 分层合成 | 0 | Apache-2.0 | — |
| ② | [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | 语音备忘录 → 1080×1920 动画 Short：逐词字幕 + 自动配乐 | 16 | MIT | — |
| ② | [xianyu110/ecommerce-video-skills](https://github.com/xianyu110/ecommerce-video-skills) | 12 个电商短视频 skills：钩子/分镜/配音/字幕/成片（中文） | 35 | MIT | — |
| ② | [kevinbadi/open-edits](https://github.com/kevinbadi/open-edits) | 「OPEN VIDEO EDIT」：raw talking-head → 成片的 AI 剪辑 harness | 34 | MIT | — |
| ② | [speechlab0210/tutorial-video-skill](https://github.com/speechlab0210/tutorial-video-skill) | 通用课程视频 skill：连贯、准确、可编辑 | 13 | MIT | — |
| ② | [chacha95/demo-video-creator](https://github.com/chacha95/demo-video-creator) | 产品 URL → 16:9 launch film（英/韩）：真实 UI 录制 + 旁白 | 8 | MIT | — |
| ② | [AmirSbss/spotlight](https://github.com/AmirSbss/spotlight) | 给 agent 网站/素材/主题，拿回一条成片短视频 | 8 | MIT | — |
| ② | [Jakeschincariol/master-skills](https://github.com/Jakeschincariol/master-skills) | 3 个 master skills：剪视频、做爆款、build anything | 5 | MIT | — |
| ② | [kmilo93sd/agent-video-editor](https://github.com/kmilo93sd/agent-video-editor) | 给 AI agent 的剪辑判断：节奏/剪切/字幕/音频/调色 | 5 | MIT | — |
| ② | [TimoteoAltobrando/ai-video-skill](https://github.com/TimoteoAltobrando/ai-video-skill) | 用 Claude Opus 5.5 制作并剪辑视频：product films、ads、talking heads | 1 | MIT | ✅ |
| ② | [vulh1209/web-video-skill](https://github.com/vulh1209/web-video-skill) | 录制 + 自动剪辑 web app 短视频（walkthrough/QA） | — | MIT | — |
| ② | [zalogarcia/claude-whiteboard-video-editor](https://github.com/zalogarcia/claude-whiteboard-video-editor) | 白板演讲剪辑：粗剪/eased zoom/调色 | — | MIT | — |
| ② | [adittaya/video-editing-skills](https://github.com/adittaya/video-editing-skills) | 30 个窄而专的剪辑 skills + presets（Apple-Standard look） | — | MIT | — |
| ② | [jamesxxx-ai/crypto-kol-video-skill](https://github.com/jamesxxx-ai/crypto-kol-video-skill) | 9:16 中文 crypto/AI explainer（Twitter KOL 用，带个人品牌） | — | MIT | — |
| ② | [emstudio010-hub/video-localize-dub](https://github.com/emstudio010-hub/video-localize-dub) | 中文短视频 → 英文配音 + 英文字幕（MiMo TTS/ASR + Remotion） | 2 | MIT | — |
| ② | [angelaosifova-ship-it/youtube-agent-improved](https://github.com/angelaosifova-ship-it/youtube-agent-improved) | 14 个 Codex skills：视频对比/开头选择/混剪 | — | MIT | — |
| ② | [misbahsy/24fps-skills](https://github.com/misbahsy/24fps-skills) | Agent skill + MCP：24fps 的 motion graphics/提示词/剪辑预设检索 | — | MIT | — |
| ② | [VisualxIntelligence/motion-tools-and-skills](https://github.com/VisualxIntelligence/motion-tools-and-skills) | AI 辅助 motion design 工具 + skills + prompts（多引擎） | — | MIT | — |
| ② | [Benitoow/cinema-skills](https://github.com/Benitoow/cinema-skills) | 给 filmmaker/editor 的 5 个 agent skills | — | MIT | — |
| ③ | [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | 教 AI「看」视频：学习、吸收、复刻、视觉反馈 | 70 | MIT | — |
| ③ | [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | 把视频和课程转成有据可查的 Agent Skill | 31 | MIT | — |
| ③ | [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | ffmpeg + 本地 Whisper 看懂本地视频（离线可用） | 9 | ⚠️ 未标注 | — |
| ③ | [tomascupr/reelql](https://github.com/tomascupr/reelql) | 视频链接 → 一份 typed JSON：章节/人物/品牌/情感弧线/逐字稿 | 28 | MIT | — |
| ③ | [0xpratzyy/dissect](https://github.com/0xpratzyy/dissect) | 把任意平台视频反向工程成可复用出片 blueprint | 24 | MIT | — |
| ③ | [Junhan2/video-lens](https://github.com/Junhan2/video-lens) | 在 Mac 上测量视频：UI 动画时序/easing 还原成 CSS | 6 | MIT | — |
| ③ | [tsingyuec/video2blog-skill](https://github.com/tsingyuec/video2blog-skill) | B 站/YouTube 视频 → 图文技术博客：抽帧 + 字幕 + 时间戳（中文） | 3 | MIT | — |
| ③ | [Jayne040622/video-to-knowledge-skill](https://github.com/Jayne040622/video-to-knowledge-skill) | 抖音/B站/小红书/YouTube → 转录 + 帧（evidence-linked） | — | MIT | — |
| ③ | [authrain-cloud-abdullahformuli/watch-skill](https://github.com/authrain-cloud-abdullahformuli/watch-skill) | 给 agent 视频输入：watch/index/ask/iterate（MCP/CLI/REST） | — | MIT | — |
| ③ | [sunsunsunai/video2tutorial-skill](https://github.com/sunsunsunai/video2tutorial-skill) | 录屏 → 图文步骤教程（DOCX）：连续关键帧抽取 | — | MIT | — |
| ④ | [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI 导演技能：剪辑理论 + Seedance/Kling/Veo 提示词语法 | 455 | CC-BY-4.0 | — |
| ④ | [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | 跨 6 个视频模型端到端出片 + 自我改进质控环 | 6 | MIT | — |
| ④ | [scenario-labs/skills](https://github.com/scenario-labs/skills) | Scenario MCP：按需选模型出图/视频/音频/3D + 驱动 Blender/Maya/Unreal | 751 | MIT | — |
| ④ | [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | 七家供应商智能路由：OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D | 2 | Apache-2.0 | — |
| ④ | [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | 11 个 skill：AI 短剧全流程（剧本 → 分镜 → 提示词 → 成片） | 2,395 | MIT | — |
| ④ | [sonlovinbot/Muse-animated-short-film](https://github.com/sonlovinbot/Muse-animated-short-film) | 在 Muse AI 上做动画短片：想法 → MP4（角色、剧本、keyframes） | 31 | MIT | — |
| ④ | [SamurAIGPT/muapi-skills](https://github.com/SamurAIGPT/muapi-skills) | Muapi 的 agent skills：一键安装（Claude Code/Cursor/Codex/Gemini CLI） | 3 | MIT | — |
| ④ | [incendies/imageat-skills](https://github.com/incendies/imageat-skills) | 官方 imageat skill：Claude Code/Codex/Cursor 生成图/视频 | — | MIT | — |
| ④ | [Saeyeon-developer/AI-video-prompt-skill](https://github.com/Saeyeon-developer/AI-video-prompt-skill) | AI 视频生产：广告分析 + Blender previs + Seedance/H3/Wan 提示词 | — | Apache-2.0 | — |
| ④ | [Isha70852/minimax-h3-remote-skill](https://github.com/Isha70852/minimax-h3-remote-skill) | MiniMax H3 Remote Colab：Ref2V/I2V/T2V | — | Apache-2.0 | — |
| ④ | [Violinet-tech/seamless-loop-video](https://github.com/Violinet-tech/seamless-loop-video) | 静帧 → 循环氛围视频（ComfyUI 内 MiniMax H3） | 2 | MIT | — |
| ④ | [MichaelCao1/Videoprompt](https://github.com/MichaelCao1/Videoprompt) | Seedance 2.5 shot-memo 风格的视频提示词 skill | 2 | MIT | — |
| ④ | [creatify-ai/creatify-ad-agent-skill](https://github.com/creatify-ai/creatify-ad-agent-skill) | Creatify Ad Agent MCP plugin：规划/生成/剪辑/发布视频广告 | — | MIT | — |

> 「5.5?」判定口径（首批 2026-09-27、第二批 2026-09-29、第三批 2026-10-07 逐仓复核各仓库 README 与描述）：**✅** = 明确点名 Opus 5.5；**—** = 未明确点名（多为通用 Claude 技能，通用即兼容 5.5）。**⚠️** = 页面未见标准许可证标识，收录前待确认。**⭐** = 抓取时的 star 快照（首批/二批 2026-09-30、第三批 2026-10-07），仅供粗筛质量参考。

## 分类明细（点标题展开）

### ① 用代码出片 —— 最贴近 Opus 5.5 的工作流

<details>
<summary><b>展开 71 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
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
| [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple-style launch films: visuals and audio share one timeline.json so they never drift。<br>Apple 风产品发布片：画面与音频共用 timeline.json 永不漂移。 | __seek(t) + headless Chrome + ffmpeg；ElevenLabs 音乐/配音/音效 | `npx skills add Dwite/launch-film -g` | MIT | — |
| [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | Disciplined pipeline: forced pre-read rules + automated QA (frozen frames / text collisions / non-determinism, qa.mjs) + original score。<br>纪律化 pipeline：强制读前置规则 + 自动 QA（冻帧/文字碰撞/非确定性检测，qa.mjs）+ 自创配乐。 | HTML 模板 + headless render + ffmpeg | 见原仓库 README | MIT | — |
| [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | Code-rendered shorts: live annotatable preview + blind-read QC (a fresh agent must restate the argument from still frames)。<br>代码短片：可标注实时预览 + 盲读质检（fresh agent 只看静帧复述论点）。 | HTML + Playwright + ffmpeg；音乐先行、按小节剪辑 | `/plugin marketplace add wcfcarolina13/motion-studio` | MIT | — |
| [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | 6-step universal pipeline: research → storyboard → TTS → Whisper word-level alignment → GSAP build → headless render。<br>6 步通用管线：调研 → 分镜 → TTS → Whisper 词级对齐 → GSAP 构建 → 无头渲染。 | HyperFrames + HTML/SVG/GSAP + whisper.cpp | 见原仓库 README | MIT | **Yes** |
| [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | Paper-collage vertical videos: torn-paper typewriter captions, photo stickers, stop-motion feel。<br>纸拼贴风竖屏视频：撕纸条打字机字幕、照片贴纸、定格感。 | HyperFrames（纯 HTML 逐帧）+ ffmpeg | `/plugin marketplace add rafiimanggala/paper-collage-skill` | MIT | — |
| [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | Reads a link to extract the brand (real UI/colors/fonts) → writes a treatment → renders film + original score from a homegrown synth。<br>给链接读品牌（真实 UI/配色/字体）→ 写导演阐述 → 出片 + 自研合成器原创配乐。 | headless Chrome + HTML + 自研 synth（80 音色）+ ffmpeg | `npx skills add Mort1d/motion-graphics-skills` | MIT | — |
| [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | Your narration + real assets (covers/screenshots used as-is) → 6 styles, 20–60s promos。<br>自己的旁白 + 真实素材（封面/截图原样使用）→ 6 种风格 20–60 秒 promo。 | 代码渲染 + ffmpeg，本地出片 | 见原仓库 README | MIT | **Yes** |
| [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | Talking-head choreography: titles/cards/app windows/bilingual captions + Chromium frame-by-frame MP4 export; ⚠ some templates still being uploaded。<br>真人口播编排：标题/卡片/软件窗口/双语字幕 + Chromium 逐帧导出 MP4；⚠ 部分模板仍在上传中。 | HTML/JS + Chromium + ffmpeg | `git clone https://github.com/adunext/adu-motion-video.git ~/.claude/skills/adu-motion-video` | MIT | — |
| [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | Outline/script → narrated MP4: 13 themes, 17 layouts, TTS + ASR round-trip verification (zh/en/yue); built for MiniMax Code。<br>大纲/脚本 → 口播 MP4：13 套主题、17 种版式，TTS + ASR 回译校验配音（中/英/粤）；为 MiniMax Code 构建。 | HTML slides + TTS + Whisper 校验 + ffmpeg | 见原仓库 README（为 MiniMax Code 构建） | MIT | — |
| [unclejobs-ai/motion-video-skill](https://github.com/unclejobs-ai/motion-video-skill) | Korean motion-graphics skill: shot order + staged-review harness for code-rendered videos; highest-starred repo of this batch。<br>韩文 motion graphics skill：出片顺序 + 分阶段检查 harness，本批 star 最高。 | 见原仓库 README（韩文文档） | `npx skills add unclejobs-ai/motion-video-skill` | MIT | — |
| [Tejashmakwana/motionmaxxing](https://github.com/Tejashmakwana/motionmaxxing) | "Looksmaxxing for motion graphics" — turns AI-looking videos into footage that feels human-made。<br>「给动态图形整容」：把 AI 味重的视频修成像人做的片子。 | 见原仓库 README | `npx skills add Tejashmakwana/motionmaxxing` | Apache-2.0 | — |
| [EGSECDA/vocaloid-style-mv-pipeline](https://github.com/EGSECDA/vocaloid-style-mv-pipeline) | Vocaloid-style hand-drawn lyric-MV production pipeline + Claude Code skill; trilingual docs。<br>Vocaloid 风手绘歌词 MV 生产管线 + Claude Code skill，日/中/英三语文档。 | 手绘 MV 管线（见原仓库 README） | `npx skills add EGSECDA/vocaloid-style-mv-pipeline` | MIT | — |
| [minosdevs/cinematic-film](https://github.com/minosdevs/cinematic-film) | Any topic → cinematic animated short with Remotion + three.js。<br>任意主题 → Remotion + three.js 电影感动画短片。 | Remotion + three.js | `npx skills add minosdevs/cinematic-film` | MIT | — |
| [ouerf-man/product-launch-motion-skill](https://github.com/ouerf-man/product-launch-motion-skill) | Pure-code product/feature launch videos with HyperFrames + GSAP。<br>纯代码产品/功能发布片：HyperFrames + GSAP。 | HyperFrames + GSAP | 见原仓库 README（skill 在子目录） | MIT | — |
| [direkturcrypto/remotion-opus-skill](https://github.com/direkturcrypto/remotion-opus-skill) | Remotion Opus skill with bundled cli/bin。<br>Remotion Opus skill，附带 cli/bin。 | Remotion | 见原仓库 README（skill 在子目录） | MIT | — |
| [Neelshah1810/Claude-Video-Skills](https://github.com/Neelshah1810/Claude-Video-Skills) | 11 skills: launch films, explainers, social ads, testimonials and more。<br>11 个 skill：launch films、explainers、social ads、testimonial 等，子目录即 skill。 | 见原仓库 README | 见原仓库 README（子目录即 skill） | MIT | — |
| [seoddhh/apple-style-promo-video-skills](https://github.com/seoddhh/apple-style-promo-video-skills) | Apple-style promo video skills。<br>Apple 风 promo 视频 skills。 | 见原仓库 README | `/plugin marketplace add seoddhh/apple-style-promo-video-skills` | MIT | — |
| [Win-Hao/knowledge-video](https://github.com/Win-Hao/knowledge-video) | One topic → 1–3 min knowledge video (fact-checked article → scenes)。<br>一个主题 → 1–3 分钟知识讲解视频（fact-checked 文章 → 场景）。 | 见原仓库 README | `/plugin marketplace add Win-Hao/knowledge-video` | MIT | — |
| [Win-Hao/code-video](https://github.com/Win-Hao/code-video) | Code-made short videos: the agent asks about your needs first, then writes a seven-block prompt。<br>用代码做短视频：agent 先问需求，再写 seven-block prompt。 | 见原仓库 README | `/plugin marketplace add Win-Hao/code-video` | MIT | — |
| [farming-labs/product-film-skill](https://github.com/farming-labs/product-film-skill) | Product launch film as a single HTML file, exported to MP4。<br>产品发布片 = 单个 HTML 文件，导出 MP4。 | 单 HTML 文件渲染 | `/plugin marketplace add farming-labs/product-film-skill` | MIT | — |
| [mos-ski/motion-video-skill](https://github.com/mos-ski/motion-video-skill) | Figma link / product URL → motion-graphics film: pulls real design tokens, beat-grid shot list, Remotion springs + jitter kit, self-critique until 8+。<br>Figma/产品 URL → 动态图形成片：拉真实设计 token、节拍网格分镜、Remotion 弹簧动效 + jitter kit，自评打分到 8+。 | Remotion + ffmpeg（jitter kit + 合成音效） | `git clone https://github.com/mos-ski/motion-video-skill ~/.claude/skills/motion-video` | MIT | — |
| [cpp285/gold-noir-video-creator](https://github.com/cpp285/gold-noir-video-creator) | Gold-noir science videos: Remotion + Three.js, 3D scenes, word-level captions, procedural score, 1080p samples included。<br>暗金风格科普视频：Remotion + Three.js、3D 场景、逐字字幕、程序合成配乐，附 1080p 示例（中文）。 | Remotion + Three.js + ffmpeg | `npx skills add cpp285/gold-noir-video-creator` | MIT | — |
| [makevoid/motion-graphics-music-video-skill-noimage](https://github.com/makevoid/motion-graphics-music-video-skill-noimage) | The noimage variant of makevoid/motion-graphics-music-video-skill (also in this list): Opus 5.5 plugin, music track + prompt only, pure code — no image models。<br>已收录 makevoid 原版的 noimage 变体：Opus 5.5 plugin，只用一条音乐 + prompt，纯代码不调用图像模型。 | Node/P5JS + ffmpeg（不调用图像模型） | `/plugin marketplace add makevoid/motion-graphics-music-video-skill-noimage` | MIT | **Yes** |
| [RohanRatwani/explainer-video-opus-5.5](https://github.com/RohanRatwani/explainer-video-opus-5.5) | Topic → motion-design explainer (YouTube 16:9 or Shorts)。<br>主题 → motion-design 讲解视频（YouTube 16:9 或 Shorts）。 | 见原仓库 README | `npx skills add RohanRatwani/explainer-video-opus-5.5` | MIT | **Yes** |
| [Everett406/code-film](https://github.com/Everett406/code-film) | Director-level code-generated video skill (Remotion), built with Claude Opus 5.5。<br>Director-level 代码生成视频 skill（Remotion），README 注明 Built with Claude Opus 5.5。 | Remotion | `npx skills add Everett406/code-film` | MIT | **Yes** |
| [lumian2015/opus-5-5-video-templates](https://github.com/lumian2015/opus-5-5-video-templates) | 30 free motion-graphics templates recreated from viral Opus 5.5 videos + one Claude Code skill。<br>30 个从 viral Opus 5.5 视频复刻的免费 motion-graphics 模板 + 一个 Claude Code skill。 | 模板库 + 代码渲染 | `npx skills add lumian2015/opus-5-5-video-templates` | MIT | **Yes** |
| [ARTHONG1/Opus-promo-Director](https://github.com/ARTHONG1/Opus-promo-Director) | Directs short beat-synced promo videos with Remotion: look-first style frames, self-review, 9:16/16:9/4:5 delivery。<br>短节拍同步 promo：look-first 风格帧 + Remotion，自审后交付 9:16/16:9/4:5。 | Remotion | `npx skills add ARTHONG1/Opus-promo-Director` | MIT | — |
| [02ui/02ui-video-copy](https://github.com/02ui/02ui-video-copy) | HyperFrames launch videos + motion library + AI-motion checks。<br>HyperFrames launch 视频 + motion library + AI 动效检查。 | HyperFrames | `npx skills add 02ui/02ui-video-copy` | MIT | — |
| [dEitY719/video-skills](https://github.com/dEitY719/video-skills) | Parameterized HyperFrames motion-graphic recipes for multiple harnesses (Claude/Codex/Gemini)。<br>参数化 HyperFrames motion-graphic recipes，多 harness（Claude/Codex/Gemini）。 | HyperFrames | `/plugin marketplace add dEitY719/video-skills` | MIT | — |
| [Saucemathis/marketing-video-skill](https://github.com/Saucemathis/marketing-video-skill) | Finished marketing videos for any brand: morphing UI, real cursors。<br>任意品牌成片营销视频：morphing UI、真实光标。 | 见原仓库 README | `npx skills add Saucemathis/marketing-video-skill` | MIT | — |
| [harish-anumula/launch-video-skill](https://github.com/harish-anumula/launch-video-skill) | Code-rendered product launch videos: story shapes + Remotion。<br>代码产品发布片：story shapes + Remotion。 | Remotion | `npx skills add harish-anumula/launch-video-skill` | MIT | — |
| [JudgePeach/remotion-shotflow](https://github.com/JudgePeach/remotion-shotflow) | Reference-guided Remotion videos: 8 shot recipes。<br>参考引导的 Remotion 视频：8 shot recipes。 | Remotion | `npx skills add JudgePeach/remotion-shotflow` | MIT | — |
| [GroMarketing/remotion-qa](https://github.com/GroMarketing/remotion-qa) | QA for Remotion videos: Reels/Shorts safe-area checks。<br>Remotion 成片 QA：Reels/Shorts 安全区检查。 | Remotion QA | `/plugin marketplace add GroMarketing/remotion-qa` | MIT | — |
| [salomonMuriel/media-production-skills](https://github.com/salomonMuriel/media-production-skills) | Director-level videos (Remotion) + scripting + AI voice-over + sound effects。<br>Director-level 视频（Remotion）+ 脚本 + AI 配音 + 音效。 | Remotion | `/plugin marketplace add salomonMuriel/media-production-skills` | MIT | — |
| [jerelvelarde/demo-skills](https://github.com/jerelvelarde/demo-skills) | Launch video + UI mockup animation skills。<br>Launch video + UI mockup 动画 skills。 | 见原仓库 README | `npx skills add jerelvelarde/demo-skills` | MIT | — |
| [KJ-AIML/product-launch-film](https://github.com/KJ-AIML/product-launch-film) | Agent skill + Remotion starter for code-rendered product launch films。<br>Agent skill + Remotion starter：代码渲染产品发布片。 | Remotion | `npx skills add KJ-AIML/product-launch-film` | MIT | — |
| [Anann99/launch-film-skill](https://github.com/Anann99/launch-film-skill) | Website + real product → expert-grade launch film。<br>网站 + 真实产品 → expert-grade launch film。 | 见原仓库 README | `/plugin marketplace add Anann99/launch-film-skill` | MIT | — |
| [NDilanka/openvids](https://github.com/NDilanka/openvids) | Remotion launch-style product videos + procedural score。<br>Remotion launch 风产品视频 + 程序配乐。 | Remotion | `npx skills add NDilanka/openvids` | MIT | — |
| [JBJMLLC/demo-studio](https://github.com/JBJMLLC/demo-studio) | Story-first product demos: composable skills + browser recording + voice-over。<br>Story-first 产品 demos：可组合 skills + 浏览器录制 + 旁白。 | 浏览器录制 + 代码渲染 | `/plugin marketplace add JBJMLLC/demo-studio` | MIT | — |
| [q2522879285-source/code-music-video-skill](https://github.com/q2522879285-source/code-music-video-skill) | Deterministic music-driven code videos: workflow + timeline validation。<br>确定性音乐驱动代码视频：workflow + 时间轴校验。 | 代码渲染 + 时间轴校验 | `npx skills add q2522879285-source/code-music-video-skill` | MIT | — |
| [patt-rick/app-promo-motion](https://github.com/patt-rick/app-promo-motion) | Motion-graphics app promo with real UI (Remotion)。<br>真实 UI 的 motion-graphics app promo（Remotion）。 | Remotion | `npx skills add patt-rick/app-promo-motion` | MIT | — |
| [WizerdBaChe/motion-video-skill](https://github.com/WizerdBaChe/motion-video-skill) | Code-rendered videos (ads / product tours / showreels)。<br>代码渲染视频（ads/product tours/showreels）。 | 见原仓库 README | 见原仓库 README（skill 在子目录） | MIT | — |
| [authrain-cloud-abdullahformuli/explainer-video-skills](https://github.com/authrain-cloud-abdullahformuli/explainer-video-skills) | Explainer-video skills: script / storyboard / rendered voice-over。<br>explainer 视频 skills：脚本/分镜/渲染旁白。 | 见原仓库 README | `/plugin marketplace add authrain-cloud-abdullahformuli/explainer-video-skills` | MIT | — |
| [yuchenmax88-wq/lingcut-video-skill](https://github.com/yuchenmax88-wq/lingcut-video-skill) | AI film pipeline: LingCut + LibTV + ffmpeg, tail-frame continuation method。<br>AI 影视流水线：LingCut + LibTV + ffmpeg，尾帧接续法（中文）。 | LingCut + LibTV + ffmpeg | `npx skills add yuchenmax88-wq/lingcut-video-skill` | MIT | — |
| [Annie-246/tabcom-skills](https://github.com/Annie-246/tabcom-skills) | Carousel, video edit and social QA video skills。<br>carousel、video edit、social QA video skills。 | 见原仓库 README | `/plugin marketplace add Annie-246/tabcom-skills` | MIT | — |
| [zeana9658-alt/remotion-particle-film](https://github.com/zeana9658-alt/remotion-particle-film) | 60-second procedural particle film + Codex skill。<br>60 秒程序粒子短片 + Codex skill。 | Remotion 粒子 | `npx skills add zeana9658-alt/remotion-particle-film` | MIT | — |
| [huynhcongdac/story-video-skill](https://github.com/huynhcongdac/story-video-skill) | AI-agent storytelling videos, 3–5 minutes (Vietnamese docs)。<br>AI agent 讲故事视频 3–5 分钟（越南语）。 | 见原仓库 README | `npx skills add huynhcongdac/story-video-skill` | MIT | — |
| [124zhe/xigua-msvideo-skill](https://github.com/124zhe/xigua-msvideo-skill) | Codex skills: YouTube curiosity stories + MS Paint storyboards + narration assembly。<br>Codex skills：YouTube 好奇心故事 + MS Paint 分镜 + 旁白组装。 | 见原仓库 README | `npx skills add 124zhe/xigua-msvideo-skill` | MIT | — |
| [jttriana86/claude-video-skill](https://github.com/jttriana86/claude-video-skill) | Code-animated videos + AI voice-over with word-level sync (Spanish)。<br>代码动画视频 + AI 配音词级同步（西语）。 | 代码渲染 + TTS 词级同步 | 见原仓库 README（skill 在子目录） | MIT | — |
| [Kianzzz/xilo-opus-video](https://github.com/Kianzzz/xilo-opus-video) | General-purpose: idea/article/reference video → multiple plan previews → finished film。<br>通用型：想法/文章/参考视频 → 多套方案预览 → 成片。 | Canvas / HTML·CSS·SVG / WebGL / Three.js / Remotion / HyperFrames / Manim + 代码合成配乐 + Playwright + ffmpeg | `npx skills add Kianzzz/xilo-opus-video` | MIT | ✅ |
| [lemomo-ai/lemo-opuscar](https://github.com/lemomo-ai/lemo-opuscar) | 43 film-style catalogs (thick oil painting, Chinese ink, ukiyo-e, whiteboard explainer, etc.), generate by style name。<br>43 种影片风格图册（厚涂油画、中国水墨、浮世绘、白板讲解等），按风格名生成。 | 代码渲染 + ffmpeg | `/plugin marketplace add lemomo-ai/lemo-opuscar` | MIT | ✅ |
| [chuspeeism/dashi-animationstyle](https://github.com/chuspeeism/dashi-animationstyle) | Chinese voiceover + visuals: 15–60s, 7 art styles, captioned, exportable to CapCut。<br>中文口播配画面：15–60 秒，7 套画风（手绘笔记、复古报刊、黑底科技等），带字幕可导剪映。（LICENSE 原文为 MIT 正文，GitHub 徽标识别为 NOASSERTION） | HTML/Canvas + 无头 Chrome 逐帧截图 + ffmpeg（不用生图模型） | 见原仓库 README（根目录 SKILL.md） | MIT | ✅ |
| [alchaincyf/huashu-art-motion](https://github.com/alchaincyf/huashu-art-motion) | Art-history topics: 35 animatable art styles (cave murals to pixel games) + 9 explainer-animation formats。<br>美术史题材：35 种可动化艺术风格（洞穴壁画到像素游戏）+ 9 种解说动画讲法。 | Playwright Chromium + ffmpeg（scripts/engine/render.py 引擎），uv | `npx skills add alchaincyf/huashu-art-motion` | MIT | — |
| [WaterDJiang/Wattter_openSkills](https://github.com/WaterDJiang/Wattter_openSkills) | One-stop: idea → Chinese script + storyboard + editable source + voiced MP4; hand-drawn paper texture, retro halftone, pixel, watercolor, sand, chalk, particles, mosaic, clay look, MG & mixed styles。<br>一站式：想法 → 中文剧本 + 分镜 + 可改源码 + 带声音 MP4；覆盖手绘纸纹、复古印刷网点、像素、水彩、沙画、粉笔、粒子、马赛克、黏土外观、MG 与混合画法。 | Canvas/p5.js 逐帧绘制 + 浏览器 + MP4 + 配音脚本（film.json 单一来源） | 复制 wattter_skills/wtt-code-animation-studio/ 或 `/plugin marketplace add WaterDJiang/Wattter_openSkills` | ⚠️ 未标注 | — |
| [Vincentwei1021/mg-styles-15](https://github.com/Vincentwei1021/mg-styles-15) | 15 MG motion-design styles, ~10s each, with full prompts + source; music generated in code。<br>15 种 MG 动态设计风格，每支约 10 秒，附完整提示词和源码，配乐代码生成。⚠️ 非可安装 skill（成片 + 提示词 + 模板）。 | HTML + JS 渲染（harness/preview.html、render.mjs）+ 代码生成配乐 | 无（成片 + 提示词 + 模板，非可安装 skill） | MIT | ✅ |
| [nutllwhy/code-brand-film](https://github.com/nutllwhy/code-brand-film) | Code-generated 15s brand films: one HTML page + paused GSAP timeline, frame-by-frame via HyperFrames; original score synthesized in Python, beats on cuts。<br>用代码做 15 秒品牌宣传片：单页 HTML + GSAP 时间轴 → HyperFrames 逐帧渲染，配乐 Python 合成原创曲、节拍跟切点。<br>🎬 样片：[15 秒演示](demos/code-brand-film-15s.mp4)（用本 skill 实测渲染） | HTML + GSAP + HyperFrames + Python 合成配乐 + ffmpeg | 见原仓库 README（根目录 SKILL.md） | MIT | — |
| [imraywang/rayskills](https://github.com/imraywang/rayskills) | ray-explainer turns articles/opinions into knowledge explainer videos (vertical, 1.5–3 min, voiceover + subtitles), frames drawn frame-by-frame in canvas/JS; the repo holds 8 skills (writer, cover, knowledge base, WeChat publisher, X Articles, etc.) + /ray router。<br>ray-explainer：文章/观点 → 知识解说视频（默认竖屏 1.5–3 分钟，配音+字幕），canvas/JS 逐帧代码绘制；仓库共 8 个 skill（写作、封面、知识库、公众号、X 文章等）+ /ray 路由。<br>🎬 样片：[3 分 46 秒演示](demos/ray-explainer-demo.mp4)（帖子原视频） | canvas/JS 逐帧绘制 + TTS 配音 + ffmpeg | `npx skills add imraywang/rayskills --skill ray-explainer`（skill 在 skills/ray-explainer 子目录） | CC BY-NC 4.0（非商业） | — |

\* 页面未显示标准许可证标识，可能是自定义许可证；收录前需到原仓库确认。Page shows no standard SPDX license badge — confirm in the source repo.

> makevoid 条目的部分音频/素材走 FAL 生成，需自备 API key（约 $30 + 3M tokens / 3 分钟歌）；其余条目本地代码渲染即可。

</details>

### ② 产品片 / 成片编辑

<details>
<summary><b>展开 24 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
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
| [xianyu110/ecommerce-video-skills](https://github.com/xianyu110/ecommerce-video-skills) | 12 e-commerce short-video skills: 3s hooks, selling-point storyboards, edge-tts voice-over, subtitle styling, ffmpeg assembly, multilingual dubbing。<br>12 个电商短视频 Agent Skills：3 秒钩子、卖点分镜、edge-tts 配音、字幕花字、ffmpeg 自动成片、多语言配音（中文）。 | edge-tts + ffmpeg | `/plugin marketplace add xianyu110/ecommerce-video-skills` | MIT | — |
| [kevinbadi/open-edits](https://github.com/kevinbadi/open-edits) | "OPEN VIDEO EDIT": AI editing harness that turns raw talking-head footage into a finished cut。<br>「OPEN VIDEO EDIT」：把 raw talking-head 素材剪成成片的 AI 剪辑 harness。 | 见原仓库 README | 见原仓库 README（install.sh） | MIT | — |
| [speechlab0210/tutorial-video-skill](https://github.com/speechlab0210/tutorial-video-skill) | General tutorial-video skill: coherent, accurate, editable。<br>通用课程视频 skill：连贯、准确、可编辑。 | 见原仓库 README | 见原仓库 README（skill 在子目录） | MIT | — |
| [chacha95/demo-video-creator](https://github.com/chacha95/demo-video-creator) | Product URL → 16:9 launch film (EN/KR): real UI capture, one-take voice-over, beat-locked motion。<br>产品 URL → 16:9 launch film（英/韩）：真实 UI 录制、one-take 旁白、beat-locked 动效。 | 真实 UI 录制 + 代码动效 | `npx skills add chacha95/demo-video-creator` | MIT | — |
| [AmirSbss/spotlight](https://github.com/AmirSbss/spotlight) | Give the agent a website, some footage, or a topic — get back a finished short video。<br>给 agent 一个网站/一段素材/一个主题，拿回一条成片短视频。 | 见原仓库 README | `/plugin marketplace add AmirSbss/spotlight` | MIT | — |
| [Jakeschincariol/master-skills](https://github.com/Jakeschincariol/master-skills) | 3 master skills: edit video, make bangers, build anything。<br>3 个 master skills：剪视频、做爆款、build anything。 | 见原仓库 README | `/plugin marketplace add Jakeschincariol/master-skills` | MIT | — |
| [kmilo93sd/agent-video-editor](https://github.com/kmilo93sd/agent-video-editor) | Editing judgment for AI agents: pacing, cuts, captions, audio, color, thumbnails。<br>给 AI agent 的剪辑判断：节奏、剪切、字幕、音频、调色、缩略图。 | 见原仓库 README | `/plugin marketplace add kmilo93sd/agent-video-editor` | MIT | — |
| [TimoteoAltobrando/ai-video-skill](https://github.com/TimoteoAltobrando/ai-video-skill) | Make and edit videos with Claude Opus 5.5: product films, ads, talking heads。<br>用 Claude Opus 5.5 制作并剪辑视频：product films、ads、talking heads。 | 见原仓库 README | `npx skills add TimoteoAltobrando/ai-video-skill` | MIT | **Yes** |
| [vulh1209/web-video-skill](https://github.com/vulh1209/web-video-skill) | Record + auto-edit web-app short videos (walkthrough / QA)。<br>录制 + 自动剪辑 web app 短视频（walkthrough/QA）。 | 录屏 + 自动剪辑 | `npx skills add vulh1209/web-video-skill` | MIT | — |
| [zalogarcia/claude-whiteboard-video-editor](https://github.com/zalogarcia/claude-whiteboard-video-editor) | Whiteboard talk editing: rough cut, eased zooms, color。<br>白板演讲剪辑：粗剪/eased zoom/调色。 | 见原仓库 README | 见原仓库 README（skill 在子目录） | MIT | — |
| [adittaya/video-editing-skills](https://github.com/adittaya/video-editing-skills) | 30 narrow, focused editing skills + presets (Apple-Standard look)。<br>30 个窄而专的剪辑 skills + presets（Apple-Standard look）。 | 见原仓库 README | `npx skills add adittaya/video-editing-skills` | MIT | — |
| [jamesxxx-ai/crypto-kol-video-skill](https://github.com/jamesxxx-ai/crypto-kol-video-skill) | 9:16 Chinese crypto/AI explainers for Twitter KOLs, with personal branding。<br>9:16 中文 crypto/AI explainer（Twitter KOL 用，带个人品牌）。 | 见原仓库 README | `npx skills add jamesxxx-ai/crypto-kol-video-skill` | MIT | — |
| [emstudio010-hub/video-localize-dub](https://github.com/emstudio010-hub/video-localize-dub) | Chinese short videos → English dubbing + English subtitles (MiMo TTS/ASR + Remotion)。<br>中文短视频 → 英文配音 + 英文字幕（MiMo TTS/ASR + Remotion）。 | MiMo TTS/ASR + Remotion | 见原仓库 README（skill 在子目录） | MIT | — |
| [angelaosifova-ship-it/youtube-agent-improved](https://github.com/angelaosifova-ship-it/youtube-agent-improved) | 14 Codex skills: video comparison, hook selection, mashups。<br>14 个 Codex skills：视频对比/开头选择/混剪。 | 见原仓库 README | `npx skills add angelaosifova-ship-it/youtube-agent-improved` | MIT | — |
| [misbahsy/24fps-skills](https://github.com/misbahsy/24fps-skills) | Agent skill + MCP: search 24fps for AI motion graphics / prompts / editing presets。<br>Agent skill + MCP：24fps 的 AI motion graphics/提示词/剪辑预设检索。 | 24fps MCP 检索 | `/plugin marketplace add misbahsy/24fps-skills` | MIT | — |
| [VisualxIntelligence/motion-tools-and-skills](https://github.com/VisualxIntelligence/motion-tools-and-skills) | AI-assisted motion-design tools + skills + prompts (Three.js/GSAP/HyperFrames/Remotion)。<br>AI 辅助 motion design 工具 + skills + prompts（Three.js/GSAP/HyperFrames/Remotion）。 | Three.js/GSAP/HyperFrames/Remotion | `npx skills add VisualxIntelligence/motion-tools-and-skills` | MIT | — |
| [Benitoow/cinema-skills](https://github.com/Benitoow/cinema-skills) | 5 agent skills for filmmakers/editors。<br>给 filmmaker/editor 的 5 个 agent skills。 | 见原仓库 README | `/plugin marketplace add Benitoow/cinema-skills` | MIT | — |

</details>

### ③ 看视频 / 把视频变成 skill（相邻方向）

<details>
<summary><b>展开 10 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | Teaches your AI to watch videos — learn, absorb, imitate, or give visual feedback。<br>教 AI「看」视频：学习、吸收、复刻，或像真人一样给视觉反馈。 | 多模态视觉 + ffmpeg 抽帧 | `npx skills add Newuxtreme/watch-video-skill` | MIT | — |
| [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | Turns videos and courses into evidence-grounded Agent Skills。<br>把视频和课程转成有据可查的 Agent Skill。 | ffmpeg 抽帧 / 转写 | `npx skills add Lum1104/video-to-skill` | MIT | — |
| [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | Lets Claude watch & understand local videos via ffmpeg + local Whisper; offline, drops into `~/.claude/skills/`。<br>用 ffmpeg + 本地 Whisper 让 Claude 看懂本地视频，离线可用。 | ffmpeg + 本地 Whisper | `npx skills add Moh4696/claude-video-vision` | ⚠️ 未标注* | — |
| [tomascupr/reelql](https://github.com/tomascupr/reelql) | Any video link → one typed JSON: summary / chapters / people / brands / emotion arc / transcript。<br>任意视频链接 → 一份 typed JSON：摘要/章节/人物/品牌/情感弧线/逐字稿。 | 视频理解 API + skill | 见原仓库 README（.claude-plugin） | MIT | — |
| [0xpratzyy/dissect](https://github.com/0xpratzyy/dissect) | Reverse-engineers any video (YouTube/TikTok/Reels/X) into a reusable production blueprint, with evals。<br>把任意平台的视频反向工程成可复用的出片 blueprint，带 evals。 | 视频理解 + blueprint 输出 | `/plugin marketplace add 0xpratzyy/dissect` | MIT | — |
| [Junhan2/video-lens](https://github.com/Junhan2/video-lens) | Measure videos on macOS: UI animation timing and easing back into CSS, scene splitting。<br>在 Mac 上测量视频：UI 动画时序和 easing 还原成 CSS、场景切分。 | 帧分析 + CSS 输出 | `/plugin marketplace add Junhan2/video-lens` | MIT | — |
| [tsingyuec/video2blog-skill](https://github.com/tsingyuec/video2blog-skill) | Bilibili/YouTube video → illustrated tech blog: frame extraction + dedup, AI subtitles, verifiable transcript, timestamp links。<br>B 站/YouTube 视频 → 图文技术博客：抽帧去重 + AI 字幕 + 可核查的图-字幕原稿 + 时间戳跳转（中文）。 | 抽帧 + 转写 | `npx skills add tsingyuec/video2blog-skill` | MIT | — |
| [Jayne040622/video-to-knowledge-skill](https://github.com/Jayne040622/video-to-knowledge-skill) | Douyin/Bilibili/Xiaohongshu/YouTube → transcript + frames (evidence-linked)。<br>抖音/B站/小红书/YouTube → 转录 + 帧（evidence-linked）。 | 转录 + 抽帧 | `npx skills add Jayne040622/video-to-knowledge-skill` | MIT | — |
| [authrain-cloud-abdullahformuli/watch-skill](https://github.com/authrain-cloud-abdullahformuli/watch-skill) | Gives agents video input: watch / index / ask / iterate (MCP/CLI/REST/Python)。<br>给 agent 视频输入：watch/index/ask/iterate（MCP/CLI/REST/Python）。 | 视频输入通道（MCP/CLI/REST） | `/plugin marketplace add authrain-cloud-abdullahformuli/watch-skill` | MIT | — |
| [sunsunsunai/video2tutorial-skill](https://github.com/sunsunsunai/video2tutorial-skill) | Screen recording → illustrated step-by-step tutorial (DOCX): continuous keyframe extraction。<br>录屏 → 图文步骤教程（DOCX）：连续关键帧抽取。 | 关键帧抽取 + 文档生成 | `npx skills add sunsunsunai/video2tutorial-skill` | MIT | — |

</details>

### ④ 调用外部视频模型（非 code-to-video，特意单列）

<details>
<summary><b>展开 13 条：用途 / 渲染栈 / 安装命令 / 许可证</b></summary>
<br>

| Skill | What it does | Render stack | Install | License | Opus 5.5? |
| --- | --- | --- | --- | --- | --- |
| [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills — Murch-style dramaturgy, blocking, montage + exact prompt syntax for Seedance 2.5 / Kling 3.0 / Veo 3.1。<br>AI 导演技能：Murch 剪辑理论、走位、蒙太奇 + Seedance 2.5 / Kling 3.0 / Veo 3.1 精确提示词语法。 | 外部视频模型 API（提示词语法库） | `npx skills add smixs/visual-skills` | CC-BY-4.0 | — |
| [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 models (Seedance 2.0, Kling, Wan, Veo, OmniHuman) with a self-improving QC loop。<br>跨 6 个模型端到端出片，带自我改进的质量控制环。 | 外部视频模型 API + ffmpeg 后期 | `npx skills add 0xadvait/ai-video-skill` | MIT | — |
| [scenario-labs/skills](https://github.com/scenario-labs/skills) | Scenario MCP: smart model picking for image/video/audio/3D + expert skill teams that drive Blender/Maya/Unreal。<br>Scenario MCP：智能选模型出图/视频/音频/3D + 驱动 Blender/Maya/Unreal 的专家 skill 团队。 | Scenario MCP + DCC 软件 | 见原仓库 README | MIT | — |
| [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Smart routing across 7 providers (OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D) with cost gating。<br>七家供应商智能路由（OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D），成本门控。 | 外部模型 API | 见原仓库 README | Apache-2.0 | — |
| [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | 11 skills: full AI short-drama pipeline (source analysis → episodic scripts → storyboard → prompts → film → review)。<br>11 个 skill：AI 短剧/漫剧全流程（原著分析 → 分集剧本 → 分镜 → 提示词 → 成片 → 审查）。 | 视频生成模型 + 剪辑 | 见原仓库 README | MIT | — |
| [sonlovinbot/Muse-animated-short-film](https://github.com/sonlovinbot/Muse-animated-short-film) | Animated shorts on Muse AI — idea to MP4: characters, script, keyframes, mega prompt, editing (Vietnamese docs)。<br>在 Muse AI 上做动画短片：想法 → MP4（角色、剧本、keyframes、剪辑），越南语文档。 | Muse AI（外部平台） | `npx skills add sonlovinbot/Muse-animated-short-film` | MIT | — |
| [SamurAIGPT/muapi-skills](https://github.com/SamurAIGPT/muapi-skills) | Muapi agent skills, one-click install for Claude Code/Cursor/Codex/Gemini CLI。<br>Muapi 的 agent skills：一键安装（Claude Code/Cursor/Codex/Gemini CLI）。 | Muapi API（外部模型） | `npx skills add SamurAIGPT/muapi-skills` | MIT | — |
| [incendies/imageat-skills](https://github.com/incendies/imageat-skills) | Official imageat skill: generate images/videos from Claude Code/Codex/Cursor。<br>官方 imageat skill：Claude Code/Codex/Cursor 生成图/视频。 | imageat API | `/plugin marketplace add incendies/imageat-skills` | MIT | — |
| [Saeyeon-developer/AI-video-prompt-skill](https://github.com/Saeyeon-developer/AI-video-prompt-skill) | AI video production: ad analysis + Blender previs + prompt skills for Seedance 2.5 / MiniMax H3 / Wan / SD25 / GPT Image。<br>AI 视频生产：广告分析 + Blender previs + Seedance 2.5/MiniMax H3/Wan/SD25/GPT Image 提示词 skills。 | 外部模型提示词 + Blender previs | 见原仓库 README（多 skill 子目录） | Apache-2.0 | — |
| [Isha70852/minimax-h3-remote-skill](https://github.com/Isha70852/minimax-h3-remote-skill) | MiniMax H3 Remote Colab: Ref2V / I2V / T2V。<br>MiniMax H3 Remote Colab：Ref2V/I2V/T2V。 | MiniMax H3（外部模型 + Colab） | 见原仓库 README（skill 在子目录） | Apache-2.0 | — |
| [Violinet-tech/seamless-loop-video](https://github.com/Violinet-tech/seamless-loop-video) | Still frame → looping ambient video (MiniMax H3 inside ComfyUI)。<br>静帧 → 循环氛围视频（ComfyUI 内 MiniMax H3）。 | ComfyUI + MiniMax H3 | `npx skills add Violinet-tech/seamless-loop-video` | MIT | — |
| [MichaelCao1/Videoprompt](https://github.com/MichaelCao1/Videoprompt) | Seedance 2.5 shot-memo style video-prompt skill。<br>Seedance 2.5 shot-memo 风格的视频提示词 skill。 | Seedance 2.5 提示词 | `npx skills add MichaelCao1/Videoprompt` | MIT | — |
| [creatify-ai/creatify-ad-agent-skill](https://github.com/creatify-ai/creatify-ad-agent-skill) | Creatify Ad Agent MCP plugin: plan / generate / edit / publish video ads。<br>Creatify Ad Agent MCP plugin：规划/生成/剪辑/发布视频广告。 | Creatify API | `/plugin marketplace add creatify-ai/creatify-ad-agent-skill` | MIT | — |

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
- [Amal-David/awesome-video-skills](https://github.com/Amal-David/awesome-video-skills) —— 按模型分类的 video/motion skills 索引（Claude Code/Opus/Astra）
- [bilaldemirerr/opus-video-recipes](https://github.com/bilaldemirerr/opus-video-recipes) —— Opus 5.5 实拍：真实 MP4 + 精确 prompt + 实测 token 成本（HyperFrames + Remotion）
- [2600th/game-with-ai-starter-pack](https://github.com/2600th/game-with-ai-starter-pack) —— Opus 5.5 field guide：games/art/animation/3D/coded video prompts

前两个主要收**成片和工作流**，中间两个是**提示词合集与技术案例**，后三个是**同主题索引与实测笔记**；这里收**可安装的 skill**，分工不同。

## 贡献

欢迎 PR —— 先读 [CONTRIBUTING.md](CONTRIBUTING.md)。一句话版本：公开仓库、有可安装的 skill（`SKILL.md` 或 plugin）、能产出或处理视频、标明许可证、**只放链接不拷源码**；新增条目需同时更新 `README.md` 与 `README.en.md` 两份表格。

## 许可与免责声明

- 本索引采用 [MIT](LICENSE) 许可，仓库内不含任何第三方代码，只有链接和简短说明。
- 与 Anthropic 无关联、非官方。Claude 与 Opus 是 Anthropic PBC 的商标。
- 各条目项目保留自己的许可证，一切以原仓库为准。
