---
name: github-chinese
description: Use when working on GitHub Chinese localization, GitHub UI translation, userscript installation, or browser-side translation behavior.
---

# GitHub Chinese Localization

Source: `https://github.com/maboloshi/github-chinese`

中文注释：这是一个 GitHub 中文化用户脚本项目，重点在安装、兼容和规则维护。

Use this skill when you need to:

- translate or localize GitHub UI
- install or troubleshoot the GitHub Chinese userscript
- work with GreasyFork / Tampermonkey / Violentmonkey setup
- test local file-based userscript loading

## What I learned

- This repo is a mature userscript with two main distribution paths: GitHub and GreasyFork.
- The project cares about browser compatibility, extension permissions, and ignore-rule quality.
- Local testing depends on `file:///` require paths and extension security settings.
- The repo is as much about translation logic as it is about installation reliability.

## 中文说明

- 适合需要 GitHub 界面汉化的用户。
- 适合用 Tampermonkey / Violentmonkey / Macaque 等脚本管理器安装。
- 适合在不同浏览器中排查权限、匹配规则和本地文件引用问题。

## Best use

1. Pick the right script source (GitHub / GreasyFork).
2. Verify browser extension permissions.
3. Test on the target GitHub page.
4. Adjust ignore rules or local path settings if needed.

## Installation mental model

- GitHub source = development track.
- GreasyFork source = stable track.
- Local file mode = fast debugging / offline testing.

## 安装要点

- 先确认脚本管理器已安装。
- 再确认浏览器允许用户脚本运行。
- 若本地调试，确认 `file:///` 访问权限。
- 安装后刷新页面，再检查效果。

## Troubleshooting checklist

- Is the userscript manager installed and allowed to run scripts?
- Is local file access enabled if using `file:///`?
- Is the right build source selected for the browser?
- Are ignore rules too broad or too narrow?
- Does the page require a refresh after installation?

## 备注

- GitHub 官方页面结构会变，规则也要跟着调整。
- 不同浏览器的脚本权限设置不同，排查时要先确认浏览器类型。

## Useful references

- GitHub source: development build
- GreasyFork source: stable build
- Local debugging with `file:///` require paths

## Notes

- Prefer the repo's script and ignore-rule model over ad hoc translation.
- Keep browser compatibility in mind: Chrome, Firefox, Safari, and Android browsers differ.
- When reporting issues, include browser, script source, and the page URL.
