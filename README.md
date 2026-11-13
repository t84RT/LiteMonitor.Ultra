# <img src="./resources/screenshots/logo.png" width="28" style="vertical-align: middle; margin-top: -4px;" /> LiteMonitor.Ultra

> 基于 [LiteMonitor](https://github.com/Diorser/LiteMonitor) 的**二次开发增强版**——在轻量级 Windows 桌面/任务栏硬件监控的基础上，新增 **12 种 UI 形态**、**10 套主题**、**AI 每日热榜播报**、**214 站点热榜导航**，并内置作者署名。

[![基于](https://img.shields.io/badge/基于-LiteMonitor-blue.svg)](https://github.com/Diorser/LiteMonitor)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![.NET](https://img.shields.io/badge/.NET-8.0-512BD4.svg)](https://dotnet.microsoft.com/)
[![Platform](https://img.shields.io/badge/Windows-10%2F11-0078D6.svg)](https://dotnet.microsoft.com/)

> **Note**
>
> 本项目基于 [LiteMonitor](https://github.com/Diorser/LiteMonitor)（原作者 **Diorser**，MIT 协议）派生修改。上游项目主页：[litemonitor.cn](https://litemonitor.cn) ｜ **本项目为非官方版本，与原作者无关联。** 完整许可证见 [LICENSE](./LICENSE)，与上游的能力差异见 [NOTICE](./NOTICE.md)，架构文档见 [docs/](./docs/architecture.md)。
>
> ![派生声明](./screenshots/04-derivation-note.png)
> *上图为同类派生项目（LiteMonitorPlus）采用的「派生声明 Note」写法，本项目沿用同样的规范：一句话讲清上游来源、非官方属性，并指引 LICENSE / NOTICE / docs。*

---

## ✨ 这是什么

`LiteMonitor.Ultra` 保留原版的全部监控能力，并额外叠加一套 **Ultra 运行时**（不破坏上游核心），无需改动原版即可获得更多 UI 形态与实用工具。

### 系统监控功能（继承上游）

| 分类 | 监控指标 |
|---|---|
| 💻 处理器（CPU） | 使用率、温度、频率、功耗、风扇、水冷 |
| 🎮 显卡（GPU） | 使用率、核心温度、显存、频率、功耗、风扇（NVIDIA / AMD / Intel） |
| 💾 主机（HOST） | 内存占用、FPS、磁盘温度、主板温度、机箱风扇 |
| 🔋 电池 | 充电状态、电量、功耗、电流、电压 |
| 📀 磁盘 | 读写速度（KB/s、MB/s），自动/手动选盘 |
| 🌐 网络 | 上传下载速度，自动/手动选网卡 |
| 📈 流量统计 | 每日上传下载流量 |
| 🔌 插件系统 | 天气、股票、加密货币、代理延迟、汇率等，支持自定义插件 |
| 🔧 硬件传感器 | 查看全部系统硬件传感器数据 |

### 本项目新增能力（Ultra 运行时）

| 功能 | 说明 |
|---|---|
| 🎛 **12 种 UI 形态** | 紧凑单条、双列信息表、卡片网格、环形仪表盘、迷你折线、终端 HUD、玻璃拟态、点阵电平、AI 新闻跑马灯、极简纯文本、资讯播报条、原版竖/横屏 |
| 🎨 **10 套主题** | 暗色 / 亮色 JSON 主题 + 跟随系统 + 定时自动切换 |
| 📰 **AI 每日热榜** | 自动抓取 `tophub.today/c/ai`，任务栏嵌入 / 面板叠加 / 独立窗口三种播报 |
| 🧭 **热榜导航（214 站点）** | 内置「今日热榜」同类站点清单，搜索 / A–E 分组 / 一键打开 / 复制链接 |
| 🧰 **工具箱（8 分页）** | 系统概览、进程 TOP、磁盘网络、文本工具、截图取色、备份、快捷启动等 |
| ⌨️ **全局热键** | 7 组 `Ctrl+Alt` 快捷键直达各功能 |
| 🛡 **兼容性自检** | DPI / 多屏 / 字体回退 / 硬件降级 / 性能分档 / 虚拟机识别 |

---

## 🖼 界面预览

| 悬浮监控条（CompactBar 形态） | 原版右键菜单 | ★ Ultra 增强菜单 |
|---|---|---|
| ![悬浮监控条](./screenshots/01-monitor-bar.png) | ![原版右键菜单](./screenshots/02-base-menu.png) | ![Ultra 增强菜单](./screenshots/03-ultra-menu.png) |

- **左 — 悬浮监控条**：桌面实时硬件监控条，两行显示 CPU / GPU / 温度 / 内存 / 上下行速率，数值按阈值红黄绿报警，右侧叠加 AI 热榜播报（标题 + 排名 + 热度 + 时间）。
- **中 — 原版右键菜单**：上游 LiteMonitor（Diorser）托盘菜单，含清理内存、显示模式、监控项、主题、网速测试、监控历史、流量统计等。
- **右 — ★ Ultra 增强菜单**：本项目新增的菜单，含 12 种 UI 形态、10 套主题、AI 每日热榜、热榜导航（214 站点）、关于（作者信息）等入口。

更多形态预览见仓库内 `UI预览/` 目录（`dotnet LiteMonitor.dll --ultra-preview UI预览` 可重新生成）。

---

## 👤 作者与署名

| 角色 | 作者 | 链接 |
|---|---|---|
| **原作者 / Upstream** | **Diorser** | [github.com/Diorser/LiteMonitor](https://github.com/Diorser/LiteMonitor) |
| **二次开发 / Maintained by** | **小吴同学电气设计** (`t84RT`) | [GitHub](https://github.com/t84RT) · [个人主页](https://t84RT.github.io) · [博客园](https://www.cnblogs.com/Student-Wu-s-Electrical-Design-t84RT) · [邮箱](mailto:xiaowu112899@outlook.com) |

> **二次开发者简介**：用代码与算法重塑传统电气设计流程。专注于工控基础、PLC 编程、伺服电机调试、配电箱与控制柜设计，开发高效智能的电气计算与设计辅助工具；同时探索嵌入式 IoT 与效率工具（C# / Python / 浏览器扩展）。

软件内已内置「关于」窗口（右键菜单 → ★ Ultra 增强 → **关于 LiteMonitor.Ultra**，或热键 **`Ctrl+Alt+A`**），同时展示原作者与二次开发者信息；首次启动会以气泡提示二次开发署名。

---

## ⌨️ 热键速查

| 热键 | 动作 |
|---|---|
| `Ctrl+Alt+V` | 顺序切换 12 种 UI 形态 |
| `Ctrl+Alt+T` | 顺序切换 10 套主题 |
| `Ctrl+Alt+U` | 打开工具箱 |
| `Ctrl+Alt+N` | 打开 AI 每日热榜 |
| `Ctrl+Alt+B` | 开关任务栏 / 导航栏资讯播报 |
| `Ctrl+Alt+H` | 打开热榜导航（214 站点） |
| `Ctrl+Alt+A` | 打开「关于 LiteMonitor.Ultra」（作者信息） |

---

## 🚀 快速开始

1. 下载 Release 中的 `LiteMonitor.Ultra-成品.zip`，解压后运行 `LiteMonitor.exe`。
2. 右键托盘/窗口 → **★ Ultra 增强** 菜单，即可切换形态、主题，打开热榜、工具箱、关于等。

---

## 🛠 编译

| 项目 | 要求 |
|---|---|
| 操作系统 | Windows 10 / 11 |
| 运行时 | .NET 8 SDK |
| IDE | Visual Studio 2022 或 Rider |

```bash
git clone https://github.com/t84RT/LiteMonitor.Ultra.git
cd LiteMonitor.Ultra
dotnet build -c Release
```

输出：`bin/Release/net8.0-windows/LiteMonitor.exe`（绿色免安装，直接双击）。

---

## 📁 目录结构

```
LiteMonitor.Ultra/
├─ src/Ultra/
│  ├─ Core/        UltraRuntime（总控）、UltraConfig、UltraLog、UltraTheme、热键、兼容
│  ├─ Views/       12 种 UI 形态渲染（ViewModels / Views_1..4）
│  ├─ UI/          UltraMenu、UltraSettingsForm、HotListNavigatorForm、UltraAboutForm
│  ├─ News/        AiNewsService、HotListData（214 站点内嵌 JSON）、TaskbarNewsCast
│  └─ Tools/       工具箱、预览导出
├─ screenshots/    界面截图（本 README 引用）
├─ docs/           架构说明（architecture.md）
├─ resources/ultra_themes/   10 套内置主题
├─ NOTICE.md       与上游的能力差异
├─ ULTRA_README.md 完整功能说明书
├─ 使用说明(必读).txt  用户快速上手
├─ README.upstream.md    上游原作者（Diorser）说明
└─ README.md       本文件（GitHub 项目说明）
```

---

## 📄 开源协议

本项目基于 **MIT License**，继承原作者 **Diorser**。你可以自由使用、修改与分发，**请保留原作者与二次开发者（小吴同学电气设计 / t84RT）的署名**。

- 完整许可文本：[LICENSE](./LICENSE)
- 与上游的能力差异：[NOTICE](./NOTICE.md)
- 上游项目：[github.com/Diorser/LiteMonitor](https://github.com/Diorser/LiteMonitor)（原作者 Diorser）

---

## 🙏 致谢

- 上游项目：[LiteMonitor](https://github.com/Diorser/LiteMonitor) by **Diorser** —— 轻量、可定制的开源桌面硬件监控基石。
- 参考项目：[LiteMonitorPlus](https://github.com/mojingjing-git/LiteMonitorPlus) by **mojingjing-git** —— 派生声明规范与架构文档结构参考。
- 二次开发、维护与扩展：**小吴同学电气设计** ([t84RT](https://github.com/t84RT))。
