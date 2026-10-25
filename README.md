# 正则表达式速查表 · Regex Cheatsheet

[![Stars](https://img.shields.io/github/stars/Ezra-Zhao/regex-cheatsheet?style=social)](https://github.com/Ezra-Zhao/regex-cheatsheet/stargazers) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE) ![Languages](https://img.shields.io/badge/languages-3-blue)

Support & more: [GitHub Sponsors](https://github.com/sponsors/Ezra-Zhao) · [Gumroad — templates & workbooks I use](https://ezraflow28.gumroad.com) · [Ko-fi](https://ko-fi.com/ezra777zhao)


> 🌍 [Español](README.es.md) · [Português](README.pt.md)

一份**一页纸**的正则表达式速查表：30 个条目，每个条目只讲三件事——**它匹配什么、一条能直接复制的模式、适用场景标签**。以 PCRE / Python / JavaScript 通用语法为准，引擎有差异的地方如实注明。不灌水，不凑数。

## 面向谁

后端开发者、运维工程师、数据处理，以及每天跟日志、文本打交道的你。如果你每次写正则都要现查文档，这张表能让你把最常用的模式一次记牢。

## 怎么用

1. 直接看 **[CHEATSHEET.md](CHEATSHEET.md)** ——速查表正文，英文模式全球开发者都无压力。
2. 拿不准的模式先去 **[regex101.com](https://regex101.com/)** 在线验证：选对引擎（PCRE2 / Python / JavaScript），一条一条试。
3. 按"元字符 → 量词 → 分组 → 断言 → 实战模式 → 避坑"的顺序过一遍，实战模式直接复制改。

## 收录了什么

| 分类 | 内容 |
|---|---|
| 🔤 基础元字符 | `.` `\d` `\w` `\s` 及大写反义、`^` `$` `\b`（6 条） |
| 🔁 量词 | `*` `+` `?` `{n,m}`、贪婪 vs 懒惰（3 条） |
| 🧩 字符组与分支 | `[...]` `[^...]` `|`（3 条） |
| 📦 分组与捕获 | `(...)` 命名捕获、非捕获组、反向引用（4 条） |
| 👀 断言 | 前瞻 `(?=)` `(?!)`、后瞻 `(?<=)` `(?<!)`（4 条） |
| 🛠️ 实战模式 | 邮箱、URL、手机号、IPv4、日期、HTML 标签、去首尾空格（7 条） |
| 🔄 替换技巧 | 反向引用替换、引擎差异说明（1 条） |
| ⚠️ 避坑 | 灾难性回溯、不要用正则解析 HTML（2 条） |

所有模式均为真实有效语法，引擎差异处已如实注明。

## 引擎说明

- 默认以 **PCRE**（PHP、Nginx、`grep -P`）为基准；
- Python `re` 与 JavaScript 的差异在相关条目中注明（如后瞻、命名捕获写法）；
- 在线验证统一用 https://regex101.com/，记得切换左上角的引擎。

## 欢迎 PR

发现错误的模式、更好的写法、翻译不到位——欢迎提 Pull Request。新增条目请保持统一格式（匹配什么 / 模式 / 标签），**提交前请在 regex101 上选对应引擎验证通过**。

## 📚 更多速查表

同一作者的其他速查表，同样有中/西/葡三语版本：

- [FFmpeg 命令速查表](https://github.com/Ezra-Zhao/ffmpeg-cheatsheet) — 28 条音视频处理命令
- [Git 实战速查表](https://github.com/Ezra-Zhao/git-cheatsheet) — 30 条日常+救命命令
- [Docker 命令速查表](https://github.com/Ezra-Zhao/docker-cheatsheet) — 28 条容器命令
- [curl 命令速查表](https://github.com/Ezra-Zhao/curl-cheatsheet) — 29 条 API 调试命令
- [jq 命令速查表](https://github.com/Ezra-Zhao/jq-cheatsheet) — 30 条 JSON 处理 filter
- [终端神器速查表](https://github.com/Ezra-Zhao/terminal-superpowers-cheatsheet) — 14 个终端效率工具
- [Adobe 免费替代速查表](https://github.com/Ezra-Zhao/adobe-free-alternatives-cheatsheet) — 16 个 Adobe 免费替代品
- [退订省钱速查表](https://github.com/Ezra-Zhao/desubscribe-cheatsheet) — 10 组退订替代，年省约 $1,260
- [kubectl 命令速查表](https://github.com/Ezra-Zhao/kubectl-cheatsheet) — Kubernetes 常用命令速查
- [SQL 查询速查表](https://github.com/Ezra-Zhao/sql-cheatsheet) — 常用 SQL 查询与函数速查
- [SSH 命令速查表](https://github.com/Ezra-Zhao/ssh-cheatsheet) — 28 条 SSH 连接、密钥与隧道命令
- [Vim 命令速查表](https://github.com/Ezra-Zhao/vim-cheatsheet) — 30 条编辑、搜索替换与宏命令
- [tmux 命令速查表](https://github.com/Ezra-Zhao/tmux-cheatsheet) — 30 条会话、窗口与窗格命令
- [systemd 命令速查表](https://github.com/Ezra-Zhao/systemd-cheatsheet) — 30 条服务管理与日志命令

## License

MIT © 2026 Guangyi Zhao，详见 [LICENSE](LICENSE)。
