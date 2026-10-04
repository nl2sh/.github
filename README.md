# nl2sh organization documentation

[简体中文](README.zh-CN.md) | [English](README.md)

This repository maintains the public organization [profile](profile/README.md) and default community files. Runtime source belongs to the component repositories linked in the profile. The TUR fork tracks packaging/upstream contribution work; it is not the Agent source.

Maintain bilingual introductions and accurate project boundaries. Check descriptions against implementation: native Android runs one Rust executable; Python A2A/MCP runs on the host; Android Bridge, JADX helper and the ADB installer have distinct roles. Describe default approval and explicit bridge auto-approval separately. Do not imply UI automation works under an ordinary Termux UID.

The organization description, repository descriptions/homepages/topics and pinned repositories are GitHub settings, separate from these files. Review them alongside profile changes. Keep existing visibility and access policies; adding a profile link does not publish a private repository. `nl2sh-helper` is currently unavailable to unauthenticated GitHub API readers, so its source/docs links require repository access.

[Contribution routing](CONTRIBUTING.md) · [中文维护说明](README.zh-CN.md)
