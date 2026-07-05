# 安装与授权说明

本文是公开说明，不包含实际包内命令。具体命令以你收到的闭源包说明为准。

## 基本要求

- Windows 系统；
- 本地已经安装 MSC Marc/Mentat；
- 本地 Marc/Mentat 可以独立正常启动；
- 拥有有效 Marc/Mentat 授权；
- 使用前准备模型备份。

## 灰度试用安装流程

```text
收到闭源包
-> 解压到本地英文路径
-> 运行状态检查
-> 获取机器信息
-> 向作者申请 license
-> 把 license.json 放到 exe 同级目录下的 licenses 文件夹
-> 再次运行 license 检查
-> 开始有限工作流测试
```

建议先使用公开示例模型、备份模型或非关键模型测试。

license 的典型位置是：

```text
<包含 exe 的文件夹>\licenses\license.json
```

注意：如果 zip 解压后出现同名嵌套目录，请使用真正包含 `.exe` 的那一层目录，不要使用外层解压目录。

## 后续 GitHub Releases 流程

如果后续闭源包放到 GitHub Releases，流程会变成：

```text
下载 Windows 闭源包
-> 解压并运行状态检查
-> 发送机器信息和试用申请
-> 获取 license
-> 放到 <包含 exe 的文件夹>\licenses\license.json 后试用
```

没有有效 license 时，包只能完成有限检查，不能开放核心功能。

## 常见问题

如果安装或授权失败，请优先反馈：

- Windows 版本；
- Marc/Mentat 版本；
- 解压路径；
- 状态检查截图；
- license 检查截图；
- 错误信息文本。

请不要一开始发送完整模型文件。
