# GitHub 发布步骤

本文用于把 `showcase-public` 发布成公开 GitHub 仓库。

## 推荐仓库名

优先推荐：

```text
Marc-MCP-Assistant
```

备选：

```text
Marc-MCP-Showcase
Marc-Mentat-AI-Assistant
Marc-MCP-Trial
```

建议使用公开仓库，但只发布当前展示目录，不发布上级工作区或任何私有目录。

## 第一次发布

1. 在 GitHub 创建一个空的 public repository。
2. 不要勾选自动创建 README、license、`.gitignore`。
3. 复制仓库地址，例如：

```text
https://github.com/your-name/Marc-MCP-Assistant.git
```

4. 在本地 `showcase-public` 目录添加 remote。
5. 推送 `main` 分支。

## 绝对不要发布

- 内部研发目录；
- 私有试用包目录；
- 付费交付包目录；
- 客户交付和支持记录；
- license 管理和签发资料；
- 任何私钥、license 签发工具、客户资料、真实模型、求解结果。

## 闭源包发布方式

闭源包不要提交进 git 仓库目录。

闭源包灰度测试通过后，可以作为 GitHub Releases 资产上传，例如：

```text
MarcMCP-trial-2.5.0-windows.zip
```

Release 文案需要说明：

- Windows only；
- closed-source package；
- requires local license；
- contact author for trial/pro license；
- no Marc/Mentat license included。

## 每次发布前检查

先运行公开边界扫描，确认没有把内部内容带进来。

扫描通过后再提交和推送。
