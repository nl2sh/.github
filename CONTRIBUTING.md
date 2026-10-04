# Contributing / 贡献

Choose the component that implements the behavior before opening an issue or pull request. / 提交 Issue 或 PR 前，先确认行为由哪个组件实现。

| Component / 组件 | Scope / 范围 |
| --- | --- |
| [nl2sh](https://github.com/nl2sh/nl2sh/issues) | Rust Agent, tools, TUI/Web/CLI, A2A/MCP, device safety and packaging / 原生 Agent、工具、界面、协议与打包 |
| [android-bridge](https://github.com/nl2sh/android-bridge/issues) | Accessibility, IME, Binder provider and companion installation / 无障碍、输入法、Binder 与伴侣安装 |
| [jadx-helper](https://github.com/nl2sh/jadx-helper/issues) | DEX helper build and class decompilation through app_process / DEX 构建与单类反编译 |
| nl2sh-helper | ADB connection, pairing, release cache and Web launch; use its repository if you have access / ADB 连接配对、发布缓存及 Web 启动，有权限时到其仓库反馈 |
| .github | Organization profile, shared contribution instructions and templates / 组织简介、共享贡献说明与模板 |

Read the selected repository's `AGENTS.md` and contribution guide, build from that repository's root, and use its CI validation commands. Keep Chinese and English documentation aligned. Interface changes involving native nl2sh and a companion require checking both sides. Do not add a dependency on a sibling checkout. / 阅读目标仓库的 `AGENTS.md` 与贡献指南，从其根目录构建并执行 CI 验证。同步中英文文档，涉及原生程序和伴侣的接口变更要核对两端，不依赖相邻检出目录。

For a bug, include component revision/version, Android API/ABI and caller UID, transport/backend, exact steps, expected/actual behavior, and a short redacted error. Distinguish task completion from device action success. State whether an action may have executed before a timeout. / 问题报告注明版本、Android API/ABI、调用 UID、传输/后端、复现步骤、预期/实际结果及脱敏错误。区分任务完成与设备动作成功，说明超时前操作是否可能执行。

Never include API keys, bearer tokens, pairing secrets, private SSH/signing keys, personal screen content or unredacted device/account data. Avoid changing approval rules merely to make a reproduction pass. / 不提交 API Key、Bearer 令牌、配对密码、SSH/签名私钥、个人屏幕内容或未脱敏设备/账号数据，不为通过复现而修改审批规则。
