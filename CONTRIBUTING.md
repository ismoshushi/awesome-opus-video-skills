# Contributing

Thanks for adding skills! This list has one job: point people at **installable, open-source skills that produce or process video** — nothing else.

## Hard rules

1. **Public GitHub repo.** Publicly accessible; no gists, no private repos, no dead links.
2. **Installable skill.** The repo must contain a `SKILL.md` (root or documented subfolder) or a plugin manifest (`.claude-plugin/plugin.json`). A random video script is not a skill.
3. **Video in or out.** It must produce video (MP4/WebM/frames) or process existing video.
4. **License stated.** The source repo must declare a license. No license = not "open source". (Existing ⚠️ entries are grandfathered pending confirmation; new PRs without a license are rejected.)
5. **Links only.** Never copy skill source code into this repo. One table row + fields + link — that's it. This keeps copyright risk at zero.
6. **One PR per skill.** Fill the template exactly and update the tables in **both** `README.md` and `README.en.md` (the full list lives inside the READMEs). Maintainers run the install command before merging.

## Entry template

```markdown
| [owner/repo](https://github.com/owner/repo) | One sentence: what video it outputs and how。<br>中文一句话用途。 | Stack (e.g. Remotion + Playwright + ffmpeg) | `npx skills add owner/repo` | MIT | — |
```

Column order: Skill · What it does · Render stack · Install · License · Opus 5.5?

`Opus 5.5?` = **Yes** only if the repo explicitly targets Opus 5.5.

## Maintainer checklist (before merge)

- [ ] repo opens, not archived
- [ ] `SKILL.md` / plugin manifest found
- [ ] license file present
- [ ] install command works
- [ ] description matches what the repo actually does

---

## 中文速览（贡献规则）

- 只收**公开 GitHub 仓库**，且仓库里有可安装的 `SKILL.md` 或 Claude Code plugin 清单，能**产出或处理视频**。
- 原仓库必须**标明许可证**；没有许可证不收（现有 ⚠️ 条目留待确认，新 PR 没有许可证直接拒）。
- 本仓库**只放链接和一句话说明**，绝不拷贝别人源码。
- 一个 PR 只加一个 skill，按固定字段**同时更新 README.md 与 README.en.md 两份表格**（完整列表就在首页 README 里，分类可折叠）；维护者会实际跑一遍安装命令再合并。
