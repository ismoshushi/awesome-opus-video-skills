# awesome-opus-video-skills

[中文说明](README.md)

A curated index of **open-source, installable Agent skills that make videos by writing code** — the workflow Claude Opus 5.5 is actually good at.

**The one idea behind this list:** Opus 5.5 does not render pixels natively. It *writes rendering code* — Canvas, Remotion, p5.js, GSAP — drives a headless browser frame by frame, and stitches the result with ffmpeg. The skills collected here package that pipeline so you can install one and just say: "make me a 60-second video about X".

This repo only **links** to open-source projects — no third-party source code is re-hosted. Every entry lists: what it does, render stack, install command, license, and whether it was built specifically for Opus 5.5.

## ⚡ Quick overview — all 110 skills

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
| ① | [tuzhechen2005/opus-video-skills](https://github.com/tuzhechen2005/opus-video-skills) | Hand-painted watercolor + kinetic typography, two skills, all generated in code | 33 | MIT | ✅ |
| ① | [howseen-ai/claude-motion-design](https://github.com/howseen-ai/claude-motion-design) | Pure-code motion design: deterministic seek(t) + beat-sync, remake mode | 105 | MIT | ✅ |
| ① | [makevoid/motion-graphics-music-video-skill](https://github.com/makevoid/motion-graphics-music-video-skill) | Music track + one prompt → motion-graphics MV (Opus 5.5 plugin) | 69 | MIT | ✅ |
| ① | [echris6/motion-video-kit](https://github.com/echris6/motion-video-kit) | Business-ad kit: independent critic loop + 28 launch-film methodology | 72 | MIT | — |
| ① | [Kimeur/motion-launch-videos](https://github.com/Kimeur/motion-launch-videos) | 8 skills in one: kinetic type / 3D / pixel / particles / App UI loop shorts | 4 | MIT | — |
| ① | [Dwite/launch-film](https://github.com/Dwite/launch-film) | Apple-style launch films: __seek(t) + headless Chrome + ElevenLabs | 1 | MIT | — |
| ① | [Lob0Garou/opus-visual-motion-engine](https://github.com/Lob0Garou/opus-visual-motion-engine) | Disciplined motion pipeline: automated QA + original score | 1 | MIT | — |
| ① | [wcfcarolina13/motion-studio](https://github.com/wcfcarolina13/motion-studio) | Code shorts with live annotated preview + blind-read QC | 0 | MIT | — |
| ① | [siyuanfeng636-cpu/agentic-motion-graphics](https://github.com/siyuanfeng636-cpu/agentic-motion-graphics) | 6-step pipeline: HyperFrames + GSAP + Whisper word-level alignment | 3 | MIT | ✅ |
| ① | [rafiimanggala/paper-collage-skill](https://github.com/rafiimanggala/paper-collage-skill) | Paper-collage vertical videos from HyperFrames templates | 3 | MIT | — |
| ① | [Mort1d/motion-graphics-skills](https://github.com/Mort1d/motion-graphics-skills) | Reads your link for brand → renders film + original synth soundtrack | 13 | MIT | — |
| ① | [axtonliu/video-illustrator](https://github.com/axtonliu/video-illustrator) | Your narration + real assets → 6 styles, 20–60s promos | 12 | MIT | ✅ |
| ① | [adunext/adu-motion-video](https://github.com/adunext/adu-motion-video) | Talking-head choreography: HTML/JS motion + Chromium frame-by-frame + ffmpeg | 18 | MIT | — |
| ① | [Wzdhehe/html2video-for-mcode](https://github.com/Wzdhehe/html2video-for-mcode) | HTML slides + TTS + ASR round-trip check → narrated MP4 (zh/en/yue) | 1 | MIT | — |
| ① | [unclejobs-ai/motion-video-skill](https://github.com/unclejobs-ai/motion-video-skill) | Korean motion-graphics skill: shot order + staged-review harness | 102 | MIT | — |
| ① | [Tejashmakwana/motionmaxxing](https://github.com/Tejashmakwana/motionmaxxing) | "Looksmaxxing for motion graphics": make AI-looking videos feel human-made | 76 | Apache-2.0 | — |
| ① | [EGSECDA/vocaloid-style-mv-pipeline](https://github.com/EGSECDA/vocaloid-style-mv-pipeline) | Vocaloid-style hand-drawn lyric-MV pipeline + Claude Code skill (trilingual) | 51 | MIT | — |
| ① | [minosdevs/cinematic-film](https://github.com/minosdevs/cinematic-film) | Any topic → cinematic animated short with Remotion + three.js | 21 | MIT | — |
| ① | [ouerf-man/product-launch-motion-skill](https://github.com/ouerf-man/product-launch-motion-skill) | Pure-code product/feature launch videos: HyperFrames + GSAP | 15 | MIT | — |
| ① | [direkturcrypto/remotion-opus-skill](https://github.com/direkturcrypto/remotion-opus-skill) | Remotion Opus skill with bundled cli/bin | 11 | MIT | — |
| ① | [Neelshah1810/Claude-Video-Skills](https://github.com/Neelshah1810/Claude-Video-Skills) | 11 skills: launch films, explainers, social ads, testimonials and more | 7 | MIT | — |
| ① | [seoddhh/apple-style-promo-video-skills](https://github.com/seoddhh/apple-style-promo-video-skills) | Apple-style promo video skills | 7 | MIT | — |
| ① | [Win-Hao/knowledge-video](https://github.com/Win-Hao/knowledge-video) | One topic → 1–3 min knowledge video (fact-checked) | 6 | MIT | — |
| ① | [Win-Hao/code-video](https://github.com/Win-Hao/code-video) | Code-made short videos: agent asks first, then writes a seven-block prompt | 6 | MIT | — |
| ① | [farming-labs/product-film-skill](https://github.com/farming-labs/product-film-skill) | Product launch film = one HTML file, exported to MP4 | 6 | MIT | — |
| ① | [mos-ski/motion-video-skill](https://github.com/mos-ski/motion-video-skill) | Figma/URL → Remotion motion-graphics film: beat-grid shots + self-critique 8+ | 8 | MIT | — |
| ① | [cpp285/gold-noir-video-creator](https://github.com/cpp285/gold-noir-video-creator) | Gold-noir science videos: Remotion + Three.js, word-level captions, procedural score | 3 | MIT | — |
| ① | [makevoid/motion-graphics-music-video-skill-noimage](https://github.com/makevoid/motion-graphics-music-video-skill-noimage) | noimage variant of the makevoid entry: pure code, no image models | 2 | MIT | ✅ |
| ① | [RohanRatwani/explainer-video-opus-5.5](https://github.com/RohanRatwani/explainer-video-opus-5.5) | Topic → motion-design explainer (16:9 or Shorts) | — | MIT | ✅ |
| ① | [Everett406/code-film](https://github.com/Everett406/code-film) | Director-level code video (Remotion), built with Opus 5.5 | — | MIT | ✅ |
| ① | [lumian2015/opus-5-5-video-templates](https://github.com/lumian2015/opus-5-5-video-templates) | 30 MG templates recreated from viral Opus 5.5 videos + skill | — | MIT | ✅ |
| ① | [ARTHONG1/Opus-promo-Director](https://github.com/ARTHONG1/Opus-promo-Director) | Short beat-synced promos: look-first style frames + Remotion self-review | — | MIT | — |
| ① | [02ui/02ui-video-copy](https://github.com/02ui/02ui-video-copy) | HyperFrames launch videos + motion library + AI-motion checks | — | MIT | — |
| ① | [dEitY719/video-skills](https://github.com/dEitY719/video-skills) | Parameterized HyperFrames motion-graphic recipes (multi-harness) | — | MIT | — |
| ① | [Saucemathis/marketing-video-skill](https://github.com/Saucemathis/marketing-video-skill) | Finished marketing videos for any brand: morphing UI, real cursors | — | MIT | — |
| ① | [harish-anumula/launch-video-skill](https://github.com/harish-anumula/launch-video-skill) | Code-rendered launch videos: story shapes + Remotion | — | MIT | — |
| ① | [JudgePeach/remotion-shotflow](https://github.com/JudgePeach/remotion-shotflow) | Reference-guided Remotion videos: 8 shot recipes | — | MIT | — |
| ① | [GroMarketing/remotion-qa](https://github.com/GroMarketing/remotion-qa) | QA for Remotion videos: Reels/Shorts safe-area checks | — | MIT | — |
| ① | [salomonMuriel/media-production-skills](https://github.com/salomonMuriel/media-production-skills) | Director-level videos (Remotion) + scripting + AI voice-over + SFX | — | MIT | — |
| ① | [jerelvelarde/demo-skills](https://github.com/jerelvelarde/demo-skills) | Launch video + UI mockup animation skills | — | MIT | — |
| ① | [KJ-AIML/product-launch-film](https://github.com/KJ-AIML/product-launch-film) | Agent skill + Remotion starter for product launch films | — | MIT | — |
| ① | [Anann99/launch-film-skill](https://github.com/Anann99/launch-film-skill) | Website + real product → expert-grade launch film | — | MIT | — |
| ① | [NDilanka/openvids](https://github.com/NDilanka/openvids) | Remotion launch-style product videos + procedural score | — | MIT | — |
| ① | [JBJMLLC/demo-studio](https://github.com/JBJMLLC/demo-studio) | Story-first product demos: composable skills + browser recording + voice-over | — | MIT | — |
| ① | [q2522879285-source/code-music-video-skill](https://github.com/q2522879285-source/code-music-video-skill) | Deterministic music-driven code videos: workflow + timeline validation | — | MIT | — |
| ① | [patt-rick/app-promo-motion](https://github.com/patt-rick/app-promo-motion) | Motion-graphics app promo with real UI (Remotion) | 2 | MIT | — |
| ① | [WizerdBaChe/motion-video-skill](https://github.com/WizerdBaChe/motion-video-skill) | Code-rendered videos (ads / product tours / showreels) | 1 | MIT | — |
| ① | [authrain-cloud-abdullahformuli/explainer-video-skills](https://github.com/authrain-cloud-abdullahformuli/explainer-video-skills) | Explainer-video skills: script / storyboard / rendered voice-over | 1 | MIT | — |
| ① | [yuchenmax88-wq/lingcut-video-skill](https://github.com/yuchenmax88-wq/lingcut-video-skill) | AI film pipeline: LingCut + LibTV + ffmpeg, tail-frame continuation | — | MIT | — |
| ① | [Annie-246/tabcom-skills](https://github.com/Annie-246/tabcom-skills) | Carousel, video edit and social QA video skills | — | MIT | — |
| ① | [zeana9658-alt/remotion-particle-film](https://github.com/zeana9658-alt/remotion-particle-film) | 60-second procedural particle film + Codex skill | 1 | MIT | — |
| ① | [huynhcongdac/story-video-skill](https://github.com/huynhcongdac/story-video-skill) | AI-agent storytelling videos, 3–5 minutes (Vietnamese) | 1 | MIT | — |
| ① | [124zhe/xigua-msvideo-skill](https://github.com/124zhe/xigua-msvideo-skill) | Codex skills: YouTube curiosity stories + MS Paint storyboards | 2 | MIT | — |
| ① | [jttriana86/claude-video-skill](https://github.com/jttriana86/claude-video-skill) | Code-animated videos + AI voice-over with word-level sync (Spanish) | — | MIT | — |
| ② | [browser-use/video-use](https://github.com/browser-use/video-use) | Edit videos with coding agents: cuts, captions, color, overlaid animation | 27,657 | MIT | — |
| ② | [iart-ai/motion-design-skills](https://github.com/iart-ai/motion-design-skills) | Motion-design fundamentals (timing/type/color/composition) + Remotion engine | 39 | MIT | — |
| ② | [iart-ai/youtube-video-skills](https://github.com/iart-ai/youtube-video-skills) | Audiogram / intro / outro — turn episodes into channel branding | 4 | MIT | — |
| ② | [0xsline/OpenChatCut](https://github.com/0xsline/OpenChatCut) | Conversational AI editor: Agent Skills + MCP + Remotion, multi-track timeline | 2,056 | AGPL-3.0 | — |
| ② | [cytxnyu/chuanyuntian-auto-edit-pro](https://github.com/cytxnyu/chuanyuntian-auto-edit-pro) | Talking-head full-screen stage packaging: Remotion + staged review gates | 1 | MIT | — |
| ② | [xiaolu-ai26/xiaolu-motion](https://github.com/xiaolu-ai26/xiaolu-motion) | Talking-head motion base + shot templates: transparent layers + ffmpeg compositing | 0 | Apache-2.0 | — |
| ② | [Dancan254/voiceover-video-skill](https://github.com/Dancan254/voiceover-video-skill) | Voice memo → 1080×1920 animated Short: word-level captions + auto score | 16 | MIT | — |
| ② | [xianyu110/ecommerce-video-skills](https://github.com/xianyu110/ecommerce-video-skills) | 12 e-commerce short-video skills: hooks, storyboards, dubbing, subtitles, assembly | 35 | MIT | — |
| ② | [kevinbadi/open-edits](https://github.com/kevinbadi/open-edits) | "OPEN VIDEO EDIT": raw talking-head → finished cut, AI editing harness | 34 | MIT | — |
| ② | [speechlab0210/tutorial-video-skill](https://github.com/speechlab0210/tutorial-video-skill) | General tutorial-video skill: coherent, accurate, editable | 13 | MIT | — |
| ② | [chacha95/demo-video-creator](https://github.com/chacha95/demo-video-creator) | Product URL → 16:9 launch film (EN/KR): real UI capture + voice-over | 8 | MIT | — |
| ② | [AmirSbss/spotlight](https://github.com/AmirSbss/spotlight) | Give the agent a site/footage/topic — get back a finished short video | 8 | MIT | — |
| ② | [Jakeschincariol/master-skills](https://github.com/Jakeschincariol/master-skills) | 3 master skills: edit video, make bangers, build anything | 5 | MIT | — |
| ② | [kmilo93sd/agent-video-editor](https://github.com/kmilo93sd/agent-video-editor) | Editing judgment for agents: pacing, cuts, captions, audio, color | 5 | MIT | — |
| ② | [TimoteoAltobrando/ai-video-skill](https://github.com/TimoteoAltobrando/ai-video-skill) | Make and edit videos with Claude Opus 5.5: product films, ads, talking heads | 1 | MIT | ✅ |
| ② | [vulh1209/web-video-skill](https://github.com/vulh1209/web-video-skill) | Record + auto-edit web-app short videos (walkthrough / QA) | — | MIT | — |
| ② | [zalogarcia/claude-whiteboard-video-editor](https://github.com/zalogarcia/claude-whiteboard-video-editor) | Whiteboard talk editing: rough cut, eased zooms, color | — | MIT | — |
| ② | [adittaya/video-editing-skills](https://github.com/adittaya/video-editing-skills) | 30 narrow editing skills + presets (Apple-Standard look) | — | MIT | — |
| ② | [jamesxxx-ai/crypto-kol-video-skill](https://github.com/jamesxxx-ai/crypto-kol-video-skill) | 9:16 Chinese crypto/AI explainers for Twitter KOLs, with personal branding | — | MIT | — |
| ② | [emstudio010-hub/video-localize-dub](https://github.com/emstudio010-hub/video-localize-dub) | Chinese short videos → English dubbing + subtitles (MiMo TTS/ASR + Remotion) | 2 | MIT | — |
| ② | [angelaosifova-ship-it/youtube-agent-improved](https://github.com/angelaosifova-ship-it/youtube-agent-improved) | 14 Codex skills: video comparison, hook selection, mashups | — | MIT | — |
| ② | [misbahsy/24fps-skills](https://github.com/misbahsy/24fps-skills) | Agent skill + MCP: search 24fps for motion graphics / prompts / editing presets | — | MIT | — |
| ② | [VisualxIntelligence/motion-tools-and-skills](https://github.com/VisualxIntelligence/motion-tools-and-skills) | AI-assisted motion-design tools + skills + prompts (multi-engine) | — | MIT | — |
| ② | [Benitoow/cinema-skills](https://github.com/Benitoow/cinema-skills) | 5 agent skills for filmmakers/editors | — | MIT | — |
| ③ | [Newuxtreme/watch-video-skill](https://github.com/Newuxtreme/watch-video-skill) | Teaches your AI to watch videos: learn, absorb, imitate, give feedback | 70 | MIT | — |
| ③ | [Lum1104/video-to-skill](https://github.com/Lum1104/video-to-skill) | Turns videos and courses into evidence-grounded Agent Skills | 31 | MIT | — |
| ③ | [Moh4696/claude-video-vision](https://github.com/Moh4696/claude-video-vision) | ffmpeg + local Whisper so Claude understands local videos (offline) | 9 | ⚠️ Unstated | — |
| ③ | [tomascupr/reelql](https://github.com/tomascupr/reelql) | Video link in → one typed JSON: chapters/people/brands/emotion arc/transcript | 28 | MIT | — |
| ③ | [0xpratzyy/dissect](https://github.com/0xpratzyy/dissect) | Reverse-engineers any video into a reusable production blueprint | 24 | MIT | — |
| ③ | [Junhan2/video-lens](https://github.com/Junhan2/video-lens) | Measure videos on macOS: UI animation timing/easing back into CSS | 6 | MIT | — |
| ③ | [tsingyuec/video2blog-skill](https://github.com/tsingyuec/video2blog-skill) | Bilibili/YouTube video → illustrated tech blog: frames + subtitles + timestamps | 3 | MIT | — |
| ③ | [Jayne040622/video-to-knowledge-skill](https://github.com/Jayne040622/video-to-knowledge-skill) | Douyin/Bilibili/Xiaohongshu/YouTube → transcript + frames (evidence-linked) | — | MIT | — |
| ③ | [authrain-cloud-abdullahformuli/watch-skill](https://github.com/authrain-cloud-abdullahformuli/watch-skill) | Gives agents video input: watch / index / ask / iterate (MCP/CLI/REST) | — | MIT | — |
| ③ | [sunsunsunai/video2tutorial-skill](https://github.com/sunsunsunai/video2tutorial-skill) | Screen recording → illustrated step-by-step tutorial (DOCX) | — | MIT | — |
| ④ | [smixs/visual-skills](https://github.com/smixs/visual-skills) | AI film-director skills + exact Seedance/Kling/Veo prompt syntax | 455 | CC-BY-4.0 | — |
| ④ | [0xadvait/ai-video-skill](https://github.com/0xadvait/ai-video-skill) | End-to-end generation across 6 video models + self-improving QC loop | 6 | MIT | — |
| ④ | [scenario-labs/skills](https://github.com/scenario-labs/skills) | Scenario MCP: on-demand model picking for image/video/audio/3D + Blender/Maya/Unreal expert skills | 751 | MIT | — |
| ④ | [hectorcanaimero/da-vinci](https://github.com/hectorcanaimero/da-vinci) | Smart routing across 7 providers: OpenAI / Gemini / FAL / KIE / HeyGen / ElevenLabs / Tripo3D | 2 | Apache-2.0 | — |
| ④ | [zenstory-ai/drama-skills](https://github.com/zenstory-ai/drama-skills) | 11 skills: full AI short-drama pipeline (script → storyboard → prompts → film) | 2,395 | MIT | — |
| ④ | [sonlovinbot/Muse-animated-short-film](https://github.com/sonlovinbot/Muse-animated-short-film) | Animated shorts on Muse AI: idea → MP4 (characters, script, keyframes) | 31 | MIT | — |
| ④ | [SamurAIGPT/muapi-skills](https://github.com/SamurAIGPT/muapi-skills) | Muapi agent skills, one-click install (Claude Code/Cursor/Codex/Gemini CLI) | 3 | MIT | — |
| ④ | [incendies/imageat-skills](https://github.com/incendies/imageat-skills) | Official imageat skill: generate images/videos from Claude Code/Codex/Cursor | — | MIT | — |
| ④ | [Saeyeon-developer/AI-video-prompt-skill](https://github.com/Saeyeon-developer/AI-video-prompt-skill) | AI video production: ad analysis + Blender previs + Seedance/H3/Wan prompt skills | — | Apache-2.0 | — |
| ④ | [Isha70852/minimax-h3-remote-skill](https://github.com/Isha70852/minimax-h3-remote-skill) | MiniMax H3 Remote Colab: Ref2V / I2V / T2V | — | Apache-2.0 | — |
| ④ | [Violinet-tech/seamless-loop-video](https://github.com/Violinet-tech/seamless-loop-video) | Still frame → looping ambient video (MiniMax H3 inside ComfyUI) | 2 | MIT | — |
| ④ | [MichaelCao1/Videoprompt](https://github.com/MichaelCao1/Videoprompt) | Seedance 2.5 shot-memo style video-prompt skill | 2 | MIT | — |
| ④ | [creatify-ai/creatify-ad-agent-skill](https://github.com/creatify-ai/creatify-ad-agent-skill) | Creatify Ad Agent MCP plugin: plan / generate / edit / publish video ads | — | MIT | — |

> "5.5?" criteria (first batch verified 2026-09-27, second batch 2026-09-29, third batch 2026-10-07, from each repo's README/description): **✅** = explicitly names Opus 5.5; **—** = not explicitly named (mostly generic Claude skills — generic means compatible with 5.5). **⚠️** = no standard SPDX license badge found; confirm before final inclusion. **⭐** = star snapshot at fetch time (batches 1–2 on 2026-09-30, batch 3 on 2026-10-07), for rough quality screening only.

## Category details (click to expand)

### ① Code-to-video — the core Opus 5.5 workflow

<details>
<summary><b>Expand 63 entries: what / stack / install / license</b></summary>
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

\* 页面未显示标准许可证标识，可能是自定义许可证；收录前需到原仓库确认。Page shows no standard SPDX license badge — confirm in the source repo.

> The makevoid entry generates part of its audio/assets via FAL — bring your own API key (~$30 + 3M tokens per 3-min song); everything else renders locally from code.

</details>

### ② Product videos & footage editing

<details>
<summary><b>Expand 24 entries</b></summary>
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

### ③ Watch videos / video-to-skill (adjacent)

<details>
<summary><b>Expand 10 entries</b></summary>
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

### ④ External video-model callers (kept separate on purpose)

<details>
<summary><b>Expand 13 entries</b></summary>
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
- [jacobbubu/claude-opus-5-5-js-animation-research](https://github.com/jacobbubu/claude-opus-5-5-js-animation-research) — 30 verified Opus 5.5 browser-animation case studies, ranked by X views (implementation deep-dives)
- [Amal-David/awesome-video-skills](https://github.com/Amal-David/awesome-video-skills) — video/motion skills index organized by model (Claude Code/Opus/Astra)
- [bilaldemirerr/opus-video-recipes](https://github.com/bilaldemirerr/opus-video-recipes) — Opus 5.5 field tests: real MP4s + exact prompts + measured token costs (HyperFrames + Remotion)
- [2600th/game-with-ai-starter-pack](https://github.com/2600th/game-with-ai-starter-pack) — Opus 5.5 field guide: games/art/animation/3D/coded video prompts

The first two index **outputs and workflows**; the next two are **prompt collections and case studies**; the last three are **same-topic indexes and field notes**. This repo indexes **installable skills** — different jobs.

## Contributing

PRs welcome — read [CONTRIBUTING.md](CONTRIBUTING.md). Short version: public repo, installable skill (`SKILL.md` or plugin), produces or processes video, license stated, **links only**; new entries must update the tables in **both** `README.md` and `README.en.md`.

## License & disclaimer

- This index is [MIT](LICENSE) licensed; it contains no third-party code, only links and short descriptions.
- Not affiliated with or endorsed by Anthropic. Claude and Opus are trademarks of Anthropic PBC.
- Each listed project keeps its own license — the source repo is always authoritative.
