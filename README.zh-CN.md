# Marc MCP Assistant

语言：**中文** | [English](README.md) | [日本語](README.ja.md)

Marc MCP Assistant 是一个面向 MSC Marc/Mentat 用户的 Windows 优先闭源工作流助手，目标是在受控的本地工具层中，让 Codex 或其他 AI 助手更稳定地辅助 Marc 工作流。

它不是 MSC/Hexagon 官方产品，不包含 Marc/Mentat 软件，不提供 Marc/Mentat 授权，也不能替代工程判断。

## 当前阶段

项目目前处于私有灰度试用阶段。

- 公开 GitHub：产品介绍、试用申请、安装说明、隐私说明和演示计划。
- 私有交付：Windows 闭源试用包和绑定机器的试用 license。
- GitHub Releases：暂未开放。试用包目前只通过联系作者后人工发放。

## 主要解决什么问题

很多 Marc 用户真正耗时间的地方，不只是理论本身，而是重复、易错、难追踪的工作流细节：

- 让 Codex/AI 以受控方式连接 Marc/Mentat；
- 检查本地 Marc/Mentat 环境配置；
- 整理模型检查线索；
- 记录项目操作和诊断步骤；
- 从日志和输入文件中收集求解失败线索；
- 辅助部分 `.t16` 结果提取和摘要；
- 为科研或工程工作保留更清晰的证据链。

目标是让这些本地工作流更可追踪、可复查，也更适合与 AI 一起讨论。

## 适合谁

如果你正在使用 MSC Marc/Mentat 做论文、科研或工程项目，并且遇到下面这些问题，这个工具可能适合你：

- 反复检查模型集合、link、边界、载荷或材料设置；
- 排查求解失败、exit number 或收敛问题；
- 想探索 Codex 辅助 Marc 工作流；
- 想更清楚地整理后处理和诊断证据；
- 希望把 Marc 操作过程、检查过程和结果提取过程记录下来。

## 私有试用

试用目前采用人工审核。如果你的场景适合当前版本，你可能会收到：

- Windows 闭源试用包；
- 绑定机器的试用 license 文件；
- 简短安装说明和 Codex 配置说明；
- 试用反馈模板。

试用可能限制有效期、机器、功能范围、包版本或支持范围。试用的目的，是确认这个工具能否帮助你的真实 Marc 工作流，而不是提供无限公开版本。

## 申请试用

联系方式：

- Email: `1309224565@qq.com`
- WeChat: `18169419809`

加微信请备注：

```text
Marc MCP Trial
```

首次联系建议包含：

```text
Marc/Mentat 版本：
Windows 版本：
研究或工程方向：
当前问题：
是否有 solver exit number：
是否可以提供截图或日志摘录：
需求：试用 / 单次诊断 / 月度使用 / 项目支持
```

请不要一开始发送完整模型文件。截图、简短日志摘录、脱敏后的问题描述，足够用于第一次判断。

## 收到包之后

收到私有包和 license 后，可以让 Codex 按照下面的说明帮你配置：

- [Codex 配置提示词](docs/codex-setup-prompt.md)
- [试用安装说明](docs/trial-install.md)

典型流程：

```text
收到试用包 -> 本地解压 -> 运行状态检查 -> 发送机器码
-> 收到 license.json -> 放到 exe 同级 licenses 文件夹
-> 配置 Codex MCP -> 验证 check_mcp_process_env -> 开始试用
```

## 重要边界

本项目不承诺：

- 自动保证模型正确；
- 保证模型一定收敛；
- 替代 Marc/Mentat 官方软件；
- 替代 Marc/Mentat 授权；
- 提供无限免费使用；
- 公开核心源码。

模型安全、工程假设和最终结论仍由用户负责。

## 文档

- [申请试用](docs/apply.md)
- [Codex 配置提示词](docs/codex-setup-prompt.md)
- [试用安装说明](docs/trial-install.md)
- [闭源包说明](docs/trial-package.md)
- [FAQ](docs/faq.md)
- [隐私说明](docs/privacy.md)
- [联系方式](docs/contact.md)
- [Marc 用户痛点](docs/pain-points.zh-CN.md)
- [演示计划](docs/demo-plan.md)
