# Src

个人源码工作区索引。根目录是一个**只跟踪索引文件**的 git 仓库（`README.md` + `.gitignore`）；下面每个子目录是一个独立项目，各自管理版本、分支与提交。

> 适用范围：顶层目录导航。各项目的开发说明、构建命令与硬性规则以该项目自己的 `README.md` / `AGENTS.md` 为准，本文件不重复。

## 项目一览

| 目录 | 是什么 | 主要技术 | 远端 |
|---|---|---|---|
| [`IcedReader`](https://github.com/wafbys/IcedReader) | Windows 桌面电子书阅读器：EPUB 2/3 + PDF，浅色纸、绿色版 | Tauri 2 · React 19 · Rust | [wafbys/IcedReader](https://github.com/wafbys/IcedReader) |
| [`IcedPicViewer`](https://github.com/wafbys/IcedPicViewer) | Windows 本地图片 / 视频查看器：瀑布流、压缩包展平、视频缩略图 | WinUI 3 · .NET 11（Core + WinUI 双工程） | [wafbys/IcedPicViewer](https://github.com/wafbys/IcedPicViewer) |
| [`IcedReel`](https://github.com/wafbys/IcedReel) | 视频库整理工具：逻辑目录命名、NFO 生成、单条展示与终端海报 | Go 1.27 | [wafbys/IcedReel](https://github.com/wafbys/IcedReel) |
| [`IcedSub`](https://github.com/wafbys/IcedSub) | 多源字幕搜索 / 下载 CLI：OpenSubtitles、ASSRT，可生成 TMDB / Wikidata 规范文件名 | .NET 10 | [wafbys/IcedSub](https://github.com/wafbys/IcedSub) |
| [`t66y-archiver`](https://github.com/wafbys/t66y-archiver) | 把 t66y 帖子全部分页抓成单个自包含 HTML（图片 base64 内嵌） | Python 标准库 | [wafbys/t66y-archiver](https://github.com/wafbys/t66y-archiver) |
| [`IcedUserScript`](https://github.com/wafbys/IcedUserScript) | 个人 Tampermonkey 脚本集，目前为 `cjk-mono` 全站 CJK / 等宽字体替换 | JavaScript（用户脚本） | [wafbys/IcedUserScript](https://github.com/wafbys/IcedUserScript) |
| [`singlefile-settings-HFA`](https://github.com/wafbys/singlefile-settings-HFA) | SingleFile 高保真网页存档配置，单 JSON，调整通过 git 留痕 | SingleFile 配置 | [wafbys/singlefile-settings-HFA](https://github.com/wafbys/singlefile-settings-HFA) |
| [`ea-learning`](https://github.com/wafbys/ea-learning) | 跟着《Evolutionary Architecture by Example》逐章学习 .NET 架构演进：笔记、练习、ADR | .NET 10 · Markdown | [wafbys/ea-learning](https://github.com/wafbys/ea-learning) |
| [`evolutionary-architecture-by-example`](https://github.com/evolutionary-architecture/evolutionary-architecture-by-example) | 上述课程的上游参考实现 clone，保持 `main` 干净，不提交个人笔记 | .NET | [上游仓库](https://github.com/evolutionary-architecture/evolutionary-architecture-by-example) |
| `os-01-boot-shell` | 从 BIOS 引导扇区到串口 shell 的最小 OS 阶梯（x86 + NASM + QEMU），当前只有文档 | x86 汇编 · QEMU | 本地仓库，无 remote |
| [`stamp-files`](https://github.com/wafbys/stamp-files) | 按数据库记录强制设置文件时间戳的 Windows CLI：哈希匹配、批量打戳、数据库维护 | Go 1.27 | [wafbys/stamp-files](https://github.com/wafbys/stamp-files) |

## 约定

- 根仓库只跟踪 `README.md` 与 `.gitignore`，不跟踪任何子项目文件；子项目的提交、推送、发版都在各自目录内完成。
- 子目录里的 `.git` 各自独立，根仓库不会把它们当子模块；根仓库也不配置子项目的 remote。
- `evolutionary-architecture-by-example` 是上游参考 clone，学习产物写在 `ea-learning`，两边不混。
- 各项目规则以目录内的 `AGENTS.md` 为准；本文件不复制这些规则，避免两处不一致。
- 新增、删除或重命名顶层项目时同步更新上表；不记录分支、提交号、未提交改动等易变状态。
