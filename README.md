# Orange NFS MusicEd UI (ONME)

**Orange NFS Music Editor UI** | **By: Shynian**

A music pack (MPF) editing tool for *Need for Speed: Carbon* and *Need for Speed: Most Wanted*, built with Qt 6, featuring a bilingual (English / Chinese) user interface.

---

## Features

- 🎵 **MPF Music Pack Management** — Import, export, and replace in-game MPF music packs
- 🎚️ **Event Configuration** — Manage music events and track associations
- 🌐 **Bilingual UI** — Built-in English and Chinese translations; switch languages on the fly
- 🖥️ **Graphical Interface** — Intuitive UI built with Qt Widgets

## Supported Games

| Game | Codename |
|------|----------|
| Need for Speed: Most Wanted | NFSMW |
| Need for Speed: Carbon | NFSC |

## Project Structure

```
OrangeNfsMusicEd-ONME/
├── main.cpp              # Program entry point (logging, HiDPI, single instance, exception handling)
├── MainWindow.cpp        # Main window core logic (~3500 lines)
├── MainWindow.h          # Main window class definition
├── MusicEd.pro           # Qt qmake project file
├── app.rc                # Windows version info resource script
├── resources.qrc         # Qt resource definition file
├── translations/         # Translation files
│   ├── musicprocessor_en.ts
│   └── musicprocessor_zh.ts
└── Windows/
    ├── app.rc            # Windows resource script
    └── manifest.xml      # Application manifest
```

### Requirements

- Qt 6.x (recommended 6.5+)
- MSVC 2022 or MinGW
- Python 3 (required by EALayer3 conversion scripts)


## About This Repository

This project was originally hosted under the GitHub organization **CARBON-Plus-Team**. In 2026, the organization was accidentally deleted. 

Fortunately, a complete copy of the latest source code  was preserved locally, allowing the project to be re-published here. 

## Acknowledgements

This project would not have been possible without the work of the following people. Their tools and resources form the foundation that ONME is built upon:

- **xan1242** — Original MPFmaster tool author — [xan1242/MPFmaster](https://github.com/xan1242/MPFmaster)
- **Hickle** — Helped with the tool development
- **BlueSkyWestSide** — Fixed compilation issues — [bluesky-dev12/PFDataCompiler](https://github.com/bluesky-dev12/PFDataCompiler)
- **Nicknine** — `mpftotext.py` script
- **Pasta** — MPF tutorial for reformed
- **Shad** — Helped simplify the tutorial

## License

MIT License — see [LICENSE](LICENSE) for details.

---

---

# 橘子极品飞车音乐编辑器 (ONME)

**Orange NFS MusicEd UI** | **作者：Shynian**

一款为《极品飞车：生死卡本谷》(NFS Carbon) 和《极品飞车：最高通缉》(NFS Most Wanted) 设计的音乐包 (MPF) 编辑工具，基于 Qt 6 构建，支持中英文双语界面。

---

## 功能特性

- 🎵 **MPF 音乐包管理** — 导入、导出、替换游戏内的 MPF 音乐包
- 🎚️ **事件配置** — 管理音乐事件 (Event) 与曲目关联
- 🌐 **中英双语** — 内置中英文翻译，可随时切换界面语言
- 🖥️ **图形化界面** — 基于 Qt Widgets 的直观操作界面

## 支持的游戏

| 游戏 | 版本代号 |
|------|----------|
| 极品飞车：最高通缉 (NFS Most Wanted) | NFSMW |
| 极品飞车：生死卡本谷 (NFS Carbon) | NFSC |

## 项目结构

```
OrangeNfsMusicEd-ONME/
├── main.cpp              # 程序入口（日志、高DPI、单实例、异常处理）
├── MainWindow.cpp        # 主窗口核心逻辑（约 3500 行）
├── MainWindow.h          # 主窗口类定义
├── MusicEd.pro           # Qt qmake 工程文件
├── app.rc                # Windows 版本信息资源脚本
├── resources.qrc         # Qt 资源定义文件
├── translations/         # 翻译文件
│   ├── musicprocessor_en.ts
│   └── musicprocessor_zh.ts
└── Windows/
    ├── app.rc            # Windows 资源脚本
    └── manifest.xml      # 应用程序清单
```


### 环境要求

- Qt 6.x（推荐 6.5+）
- MSVC 2022 或 MinGW
- Python 3（EALayer3 转换脚本依赖）


## 关于本仓库

本项目最初托管于 GitHub 组织 **CARBON-Plus-Team** 下。2026 年，该组织被误删除。

幸运的是，本地保留了完整的最新源码，因此得以重新发布于此。

## 致谢

没有以下这些人的工作，本项目不可能完成。他们的工具和资源构成了 ONME 赖以构建的基础：

- **xan1242** — 原始 MPFmaster 工具作者 — [xan1242/MPFmaster](https://github.com/xan1242/MPFmaster)
- **Hickle** — 协助工具开发
- **BlueSkyWestSide** — 修复编译问题 — [bluesky-dev12/PFDataCompiler](https://github.com/bluesky-dev12/PFDataCompiler)
- **Nicknine** — `mpftotext.py` 脚本
- **Pasta** — MPF 教程
- **Shad** — 帮助简化教程

## 许可证

MIT License — 详见 [LICENSE](LICENSE)

---

*Orange NFS MusicEd UI By: Shynian*
