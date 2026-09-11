<p align="center">
  <a href="https://github.com/nl2sh/nl2sh">
    <img src="https://raw.githubusercontent.com/nl2sh/nl2sh/master/assets/logo.png" alt="nl2sh logo" width="180">
  </a>
</p>

<h1 align="center">nl2sh</h1>

<p align="center">
  A safe, Android-native natural-language shell agent, built as a single Rust executable with a rich terminal UI.
</p>

nl2sh turns natural-language tasks into shell operations for stock Android `adb shell` and Termux. Every model-proposed command must pass the local `LLM → Security → Confirmation → Execution` boundary before it can run.

nl2sh 将自然语言任务转换为 Android shell 操作，以原生 `adb shell` 为一等运行环境并兼容 Termux。模型提出的每条命令都必须经过本地 `LLM → Security → Confirmation → Execution` 安全链。

- Android API 26+; AArch64 and ARMv7 release builds
- Stable Rust, ratatui/crossterm TUI, multi-round Tool Calling
- Explicit confirmation for mutations and strong confirmation for dangerous operations
- Root access never bypasses risk classification or confirmation

[Source & documentation](https://github.com/nl2sh/nl2sh) · [Releases](https://github.com/nl2sh/nl2sh/releases) · [Issues](https://github.com/nl2sh/nl2sh/issues) · [Discussions](https://github.com/nl2sh/nl2sh/discussions)
