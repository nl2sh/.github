# nl2sh 组织文档

[简体中文](README.zh-CN.md) | [English](README.md)

本仓库维护公开组织 [简介](profile/README.md) 与默认社区文件。运行时代码位于简介列出的各组件仓库。TUR fork 用于打包与上游贡献，不是 Agent 源码仓库。

同步维护双语介绍并根据实现描述项目边界：Android 运行单个 Rust 程序，Python A2A/MCP 在主机侧运行；Android Bridge、JADX helper 和 ADB 安装助手各有用途。默认审批与显式 bridge 自动审批应分别说明，不应暗示普通 Termux UID 具备完整 UI 自动化权限。

组织描述、仓库描述/主页/topics 与置顶仓库属于独立的 GitHub 设置，更新简介时一并核对。保持既有可见性与访问策略，添加简介链接不代表公开私有仓库。当前未鉴权 GitHub API 无法读取 `nl2sh-helper`，访问其源码/文档链接需要仓库权限。

[贡献与问题分流](CONTRIBUTING.md) · [English maintenance notes](README.md)
