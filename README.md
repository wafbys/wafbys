# Src

个人源码工作区索引，同时收录 `Src` 外的 `Bin` 工具箱。本仓库（`wafbys/wafbys`）是两台机器的**唯一索引**，只跟踪 `README.md` 与 `.gitignore`；本地 `Src` 根目录不再作为 git 仓库，下面每个子目录仍是独立项目，各自管理版本、分支与提交。

> 适用范围：顶层目录导航。各项目的开发说明、构建命令与硬性规则以该项目自己的 `README.md` / `AGENTS.md` 为准，本文件不重复。

## 项目一览

| 目录 | 是什么 | 主要技术 | 远端 |
|---|---|---|---|
| [`IcedReader`](https://github.com/wafbys/IcedReader) | Windows 桌面电子书阅读器：EPUB 2/3 + PDF，浅色纸、绿色版 | Tauri 2 · React 19 · Rust | [wafbys/IcedReader](https://github.com/wafbys/IcedReader) |
| [`IcedPicViewer`](https://github.com/wafbys/IcedPicViewer) | Windows 本地图片 / 视频查看器：瀑布流、压缩包展平、视频缩略图 | WinUI 3 · .NET 11（Core + WinUI 双工程） | [wafbys/IcedPicViewer](https://github.com/wafbys/IcedPicViewer) |
| [`SavorReader`](https://github.com/wafbys/SavorReader) | Windows 本地 EPUB/PDF 书库与阅读器：WebView2 渲染、SQLite 书库 | WinUI 3 · .NET 11（Core + WinUI 双工程） | [wafbys/SavorReader](https://github.com/wafbys/SavorReader) |
| `IcedReel` | 视频库整理工具：逻辑目录命名、NFO 生成、单条展示与终端海报 | Go 1.27 | 私有 |
| [`IcedSub`](https://github.com/wafbys/IcedSub) | 多源字幕搜索 / 下载 CLI：OpenSubtitles、ASSRT，可生成 TMDB / Wikidata 规范文件名 | .NET 10 | [wafbys/IcedSub](https://github.com/wafbys/IcedSub) |
| `t66y-archiver` | 把 t66y 帖子全部分页抓成单个自包含 HTML（图片 base64 内嵌） | Python 标准库 | 私有 |
| [`IcedUserScript`](https://github.com/wafbys/IcedUserScript) | 个人 Tampermonkey 脚本集，目前为 `cjk-mono` 全站 CJK / 等宽字体替换 | JavaScript（用户脚本） | [wafbys/IcedUserScript](https://github.com/wafbys/IcedUserScript) |
| [`singlefile-settings-HFA`](https://github.com/wafbys/singlefile-settings-HFA) | SingleFile 高保真网页存档配置，单 JSON，调整通过 git 留痕 | SingleFile 配置 | [wafbys/singlefile-settings-HFA](https://github.com/wafbys/singlefile-settings-HFA) |
| `ea-learning` | 跟着《Evolutionary Architecture by Example》逐章学习 .NET 架构演进：笔记、练习、ADR | .NET 10 · Markdown | 私有 |
| [`evolutionary-architecture-by-example`](https://github.com/evolutionary-architecture/evolutionary-architecture-by-example) | 上述课程的上游参考实现 clone，保持 `main` 干净，不提交个人笔记 | .NET | [上游仓库](https://github.com/evolutionary-architecture/evolutionary-architecture-by-example) |
| `os-01-boot-shell` | 从 BIOS 引导扇区到串口 shell 的最小 OS 阶梯（x86 + NASM + QEMU），当前只有文档 | x86 汇编 · QEMU | 本地仓库，无 remote |
| [`stamp-files`](https://github.com/wafbys/stamp-files) | 按数据库记录强制设置文件时间戳的 Windows CLI：哈希匹配、批量打戳、数据库维护 | Go 1.27 | [wafbys/stamp-files](https://github.com/wafbys/stamp-files) |
| `winconfig` | Windows 11 开发环境基线脚本：固定目录、固定版本、固定换行策略 | PowerShell 7 · winget | 私有 |

## 工具仓库

`Bin` 不在 `Src` 下，单独列出。

| 目录 | 是什么 | 主要技术 | 远端 |
|---|---|---|---|
| `Bin`（`C:\Users\YF\Bin`） | Windows 日常工具箱：媒体整理、字体安装、网页文章存档、目录备份、OpenCode 更新 | Python · PowerShell · Bash | [wafbys/Bin](https://github.com/wafbys/Bin) |

## 约定

- 本索引仓库只跟踪 `README.md` 与 `.gitignore`，不跟踪任何子项目文件；本地 `Src` 根目录不再是 git 仓库。
- `Bin` 不在 `Src` 下，单独列在「工具仓库」；文件与提交仍由 `Bin` 仓库自己管理，本仓库只维护索引。
- 两台机器都以本仓库的 README 为索引；本地 `Src/README.md` 已弃用，不再更新。
- 私有仓库在表中只保留名称，远端列标「私有」，不提供链接。
- 子目录里的 `.git` 各自独立，本索引仓库不会把它们当子模块，也不配置子项目的 remote。
- `evolutionary-architecture-by-example` 是上游参考 clone，学习产物写在 `ea-learning`，两边不混。
- 各项目规则以目录内的 `AGENTS.md` 为准；本文件不复制这些规则，避免两处不一致。
- 新增、删除或重命名顶层项目时同步更新上表；不记录分支、提交号、未提交改动等易变状态。
