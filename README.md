# Marc MCP Assistant

面向 MSC Marc/Mentat 用户的 AI 辅助工作流工具。

它的目标不是替代 Marc/Mentat，也不是自动保证模型正确，而是让 Codex/AI 在受控工具层下，帮助用户处理 Marc 工作流里重复、易错、难追踪的部分。

当前阶段：**Windows 闭源灰度试用**。

> This is an independent closed-source workflow assistant for MSC Marc/Mentat users. It is not an official MSC/Hexagon product.

## 能解决什么问题

很多 Marc 用户真正卡住的地方，不一定是理论，而是这些反复消耗时间的工作流细节：

- 想让 Codex/AI 辅助 Marc/Mentat，但缺少稳定、受控的连接方式。
- Mentat 里的模型检查、集合检查、link 检查、边界和载荷检查很重复。
- 求解失败后，日志、输入文件和错误线索分散，排查成本高。
- `.t16` 后处理经常需要手动导出、整理、记录。
- 论文、科研和工程项目需要留下清楚证据：改了什么、检查了什么、提取了什么结果。

Marc MCP Assistant 试图把这些事情组织成可记录、可复查、可逐步自动化的本地工作流。

## 当前能力范围

闭源包当前主要面向 Windows + 本地 Marc/Mentat 环境，设计能力包括：

- 本地 Marc/Mentat 环境检查；
- Codex/AI 与 Marc 工作流的受控 MCP 连接；
- 项目化操作记录；
- Mentat 会话辅助流程；
- 模型集合、link、边界、载荷等检查线索整理；
- 求解输入、日志和失败线索整理；
- 部分 `.t16` 结果提取和摘要；
- 面向诊断和支持的反馈流程。

具体能力会随版本和 license 类型变化。

## 试用方式

目前先不公开发放可用授权。流程是：

```text
查看本页面
-> 联系作者，说明 Marc 版本和当前痛点
-> 通过后获取 Windows 闭源包和本地试用 license
-> 在本机运行检查命令
-> 试用有限工作流
-> 反馈问题或转为付费使用
```

闭源包会先经过真实用户灰度测试。确认安装、授权和基本流程稳定后，后续会考虑放到 GitHub Releases，用户可自行下载包，再联系作者申请试用 license。

试用不是无限公开版本，可能限制：

- 使用时间；
- 绑定机器；
- 功能范围；
- 运行次数；
- 支持的 Marc 版本；
- 高级诊断和批处理能力。

## 联系试用

Email: `1309224565@qq.com`

WeChat: `18169419809`

加微信请备注：

```text
Marc MCP Trial
```

首次联系请尽量只发简短信息：

```text
Marc 版本：
Windows 版本：
研究/工程方向：
当前最想解决的问题：
是否有求解报错、exit number、日志或截图：
```

一开始不要直接发送完整模型文件。

## 适合谁

适合正在使用 MSC Marc/Mentat 做论文、科研或工程模型，并且被以下问题困扰的用户：

- 重复建模检查；
- 求解报错和收敛排查；
- Mentat 操作流程复现；
- `.t16` 后处理整理；
- 想探索 Codex/AI 辅助 Marc 工作流；
- 希望把项目中的模型操作和结果提取过程记录清楚。

## 不承诺什么

为了避免误解，当前版本不承诺：

- 不替代 Marc/Mentat 官方软件；
- 不提供 Marc/Mentat 授权；
- 不保证任何模型一定收敛；
- 不保证自动修复所有建模错误；
- 不默认收集或上传用户模型；
- 不公开核心源码。

## 更多说明

- [试用申请](docs/apply.md)
- [试用流程](docs/trial.md)
- [安装与授权说明](docs/trial-install.md)
- [闭源包说明](docs/trial-package.md)
- [第一位灰度用户测试清单](docs/first-beta-test.zh-CN.md)
- [GitHub 发布步骤](docs/github-publish.zh-CN.md)
- [GitHub 仓库设置建议](docs/repository-settings.zh-CN.md)
- [FAQ](docs/faq.md)
- [隐私说明](docs/privacy.md)
- [演示计划](docs/demo-plan.md)
- [公开发布检查清单](docs/public-release-checklist.md)

## English Summary

Marc MCP Assistant is a Windows-first, closed-source workflow assistant for MSC Marc/Mentat users. It aims to help with controlled AI-assisted Marc workflows, environment checks, model-inspection traces, solver-diagnosis organization, and selected `.t16` post-processing tasks.

Trial access is manual and license-bound. Please contact the author with your Marc version, Windows version, research/engineering field, and current pain point.
