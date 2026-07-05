# Marc MCP Assistant

语言：**中文** | [English](README.md) | [日本語](README.ja.md)

Marc MCP Assistant 是一个面向 MSC Marc/Mentat 用户的 Windows 优先闭源工作流助手。它的目标是在受控的本地环境中，通过 MCP 把 Codex 或其他 AI 助手连接到 Marc 工作流，让模型检查、求解诊断线索、结果提取和过程记录变得更清晰、更可追踪。

它不是 MSC/Hexagon 官方产品，不包含 Marc/Mentat 软件，不提供 Marc/Mentat 授权，也不能替代工程判断。

## 当前版本进度

```text
当前私有试用线：MarcMCP trial 2.5.0-trial
平台：Windows
阶段：私有 beta
分发方式：先联系作者，再私有发放闭源包和试用 license
使用方式：本地 MSC Marc/Mentat + Codex MCP
GitHub 公开 Release：暂未开放
```

当前版本已经可以进行有指导的私有试用。新功能仍在持续开发中，也欢迎真实 Marc/Mentat 用户提出问题、建议和使用反馈。

## 当前版本已支持

当前闭源包重点支持这些实际工作：

- 启动受控的本地 MCP server，让 Codex 连接本地 Marc/Mentat 工作流；
- 检查 package 状态和 license 状态；
- 显示申请试用 license 所需的机器码；
- 验证 Codex 使用的是当前交付的闭源包路径，而不是旧包、错误路径或开发路径；
- 检查本地 MSC Marc/Mentat 环境是否能被识别；
- 初始化本地 Marc 项目工作区，用于后续辅助流程；
- 运行基础 MCP doctor 和环境检查；
- 辅助整理模型检查线索，例如 set、link、边界、载荷、材料等；
- 辅助从日志、输入文件和 exit number 中收集求解失败线索；
- 辅助部分 `.t16` 结果提取和摘要流程；
- 为论文、科研和工程项目保留更清晰的检查、修改和结果证据链；
- 当需要支持或诊断时，提供更结构化的反馈路径。

## 它主要解决什么问题

很多 Marc 用户真正耗时的地方，不只是理论本身，而是重复、易错、难追踪的工作流细节。这个项目希望减少：

- Mentat 模型细节反复手工检查；
- 不清楚 Codex 当前到底连接了哪个 exe、哪个包、哪个工作流；
- 求解失败后，日志、输入文件、截图、错误线索分散在不同地方；
- 后处理记录依赖手工整理，后续难以复查；
- 论文或工程项目中难以说明“检查了什么、改了什么、提取了什么”；
- Marc 问题很难清楚地交给 AI 助手或支持人员一起讨论。

目标不是让 Marc 自动化一切，而是让本地 Marc 工作流更可控、更可追踪、更容易复查，也更适合和 AI 一起讨论。

## 持续开发中

后续会继续推进：

- 覆盖更多 Marc/Mentat 工作流；
- 改进求解失败诊断模板；
- 增加常见 `.t16` 后处理辅助能力；
- 完善中文、英文、日文说明；
- 优化试用、反馈、支持和版本更新流程；
- 根据真实用户问题持续升级闭源包。

如果你的研究方向或工程方向有特殊的 Marc/Mentat 工作流，欢迎提出建议。真实用户的问题，是后续功能迭代最重要的输入。

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

收到私有包和 license 后，可以让 Codex 按照下面的说明帮助你配置：

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
- 公开核心源代码。

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
