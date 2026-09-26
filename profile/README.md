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
- Optional host-side A2A 1.0 gateway and stdio MCP adapter for device inspection and Agent consultation
- Explicit confirmation for mutations and strong confirmation for dangerous operations
- Root and unattended A2A/MCP calls cannot bypass local risk classification or confirmation

[Source & documentation](https://github.com/nl2sh/nl2sh) · [A2A/MCP gateway](https://github.com/nl2sh/nl2sh/tree/master/a2a_gateway) · [Releases](https://github.com/nl2sh/nl2sh/releases) · [Issues](https://github.com/nl2sh/nl2sh/issues) · [Discussions](https://github.com/nl2sh/nl2sh/discussions)
