<p align="center">
  <a href="https://github.com/nl2sh/nl2sh">
    <img src="https://raw.githubusercontent.com/nl2sh/nl2sh/master/assets/logo.png" alt="nl2sh logo" width="180">
  </a>
</p>

<h1 align="center">nl2sh</h1>

<p align="center">
  An Android-native AI shell agent with a Rust TUI, embedded Web workspace, and local safety approvals.
</p>

nl2sh turns natural-language tasks into device actions for stock Android `adb shell` and Termux. The Android runtime is a single Rust executable with a terminal UI, browser sessions, and bounded built-in tools. Actions pass local risk assessment and require confirmation when the operation warrants it.

nl2sh 将自然语言任务转换为 Android 设备操作，以原生 `adb shell` 为一等运行环境并兼容 Termux。单个 Rust 可执行文件内置终端界面、Web 多会话和有界工具；命令及其他操作均经过本地风险评估与确认。

- Android API 26+; AArch64 and ARMv7 release builds
- Stable Rust, ratatui/crossterm TUI, embedded Web UI, multi-round Tool Calling
- Structured file, Android diagnostics, UI, network, audio, and chart tools
- Optional host-side A2A 1.0 JSON-RPC gateway, Streamable HTTP and stdio MCP for direct device tools, screenshots and optional Agent consultation
- Explicit confirmation for mutations and strong confirmation for dangerous operations
- Root never skips risk assessment. Bridge writes need device-local approval by default; explicit `bridge_auto_approve = true` permits unattended bridge actions at every risk level while retaining validation and risk assessment.

[Source & documentation](https://github.com/nl2sh/nl2sh) · [A2A/MCP gateway](https://github.com/nl2sh/nl2sh/tree/master/a2a_gateway) · [Releases](https://github.com/nl2sh/nl2sh/releases) · [Issues](https://github.com/nl2sh/nl2sh/issues) · [Discussions](https://github.com/nl2sh/nl2sh/discussions)

## Projects / 项目

| Repository | Purpose / 用途 | Documentation / 文档 |
| --- | --- | --- |
| [nl2sh](https://github.com/nl2sh/nl2sh) | Rust device Agent, TUI/Web/CLI and host A2A/MCP gateway / 设备 Agent 与主机协议网关 | [中文](https://nl2sh.github.io/nl2sh/) · [English](https://nl2sh.github.io/nl2sh/en/) |
| [android-bridge](https://github.com/nl2sh/android-bridge) | Optional shell/root-only Accessibility and Unicode keyboard companion / 无障碍及 Unicode 键盘伴侣 | [中文](https://github.com/nl2sh/android-bridge/blob/main/docs/zh/guide.md) · [English](https://github.com/nl2sh/android-bridge/blob/main/docs/en/guide.md) |
| [jadx-helper](https://github.com/nl2sh/jadx-helper) | Single-DEX class decompiler run with Android app_process / 单类反编译 DEX 工具，不作为 APK 安装 | [中文](https://github.com/nl2sh/jadx-helper/blob/main/docs/zh/guide.md) · [English](https://github.com/nl2sh/jadx-helper/blob/main/docs/en/guide.md) |
| [nl2sh-helper](https://github.com/nl2sh/nl2sh-helper) | Android ADB installer and Web launcher / Android ADB 安装与 Web 启动助手 | [中文](https://github.com/nl2sh/nl2sh-helper/blob/main/docs/zh/guide.md) · [English](https://github.com/nl2sh/nl2sh-helper/blob/main/docs/en/guide.md) |

辅助项目独立构建与发布，不是主仓库的必需依赖。Android UI 自动化需要 shell/root 权限；Termux 普通应用 UID 的权限并不等同于 ADB shell。A2A/MCP 默认沿用设备端审批；显式启用 `bridge_auto_approve` 后桥接调用可自动批准所有风险等级，令牌仅应交给完全可信的客户端。内置 Web 当前无需登录并监听所有 IPv4 接口，应在可信网络使用。

The auxiliary projects build and release independently. Device deployment remains a single Rust executable; Python runs only on the optional gateway host. Read each project's guide for installation, permissions and release verification. The built-in Web listener currently has no login and binds all IPv4 interfaces; use a trusted network.

`nl2sh-helper` source and documentation currently require repository access. / `nl2sh-helper` 源码与文档当前需要仓库访问权限。
