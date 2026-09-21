# Orange NFS MusicEd UI (ONME)

**橘子极品飞车音乐编辑器** | **作者：Shynian**

一款为《极品飞车：生死卡本谷》(NFS Carbon) 和《极品飞车：最高通缉》(NFS Most Wanted) 设计的音乐包 (MPF) 编辑工具，基于 Qt 6 构建，支持中英文双语界面。

---

## 功能特性

- 🎵 **MPF 音乐包管理** — 导入、导出、替换游戏内的 MPF 音乐包
- 🔊 **EALayer3 音频转换** — 内置 EALayer3 格式编解码，支持游戏音频与通用格式互转
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
├── MainWindow.cpp        # 主窗口核心逻辑（~3500 行）
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

## 编译说明

### 环境要求

- Qt 6.x（推荐 6.5+）
- MSVC 2022 或 MinGW
- Python 3（EALayer3 转换脚本依赖）

### 编译步骤

```bash
# 使用 qmake
qmake MusicEd.pro
nmake        # MSVC
# 或
make         # MinGW
```

> **注意**：`resources.qrc` 引用了 `tools/` 目录下的辅助工具（`MPFmaster.exe`、`sx.exe`、`ffmpeg.exe` 等）。这些工具属于第三方二进制文件，未包含在本仓库中。编译时请将所需工具放入 `tools/` 目录，或修改 `resources.qrc` 移除相关引用。

### 中文路径问题

MSVC 的资源编译器 (`rc.exe`) 不支持中文路径。如果项目路径含中文，可使用 `subst` 映射为英文盘符：

```cmd
subst X: "C:\path\to\project"
```

## 关于本仓库

本项目最初托管于 GitHub 组织 **CARBON-Plus-Team** 下。2026 年，该组织被误删除，由于账户未订阅付费支持服务，GitHub 官方无法协助恢复组织及其下的仓库。

幸运的是，本地保留了完整的最新源码（最后修改于 2026 年 7 月），因此得以重新发布于此。本次重新上传仅包含具有学习价值的源代码，不含编译产物、第三方工具二进制及图标等资源文件。

## 许可证

MIT License — 详见 [LICENSE](LICENSE)

---

*Orange NFS MusicEd UI By: Shynian*
