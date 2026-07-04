# 公开发布检查清单

发布 GitHub 公开页、GitHub Release 或社交平台内容前，先检查本页。

## GitHub 仓库

- 仓库只包含公开说明、演示材料、申请入口和脱敏资料。
- 不包含核心源码。
- 不包含内部脚本、MCP 实现、license 签发工具或私钥。
- 不包含客户资料、真实模型、求解结果、内部路线图。
- 不包含本地绝对路径。
- 不包含真实 license 文件。
- 不包含 Marc/Mentat 授权文件。
- README 明确说明闭源、Windows 优先、非官方 MSC/Hexagon 产品。

## GitHub Releases

闭源包如果后续放到 GitHub Releases，需要单独检查：

- Release 里只放可公开下载的闭源包，不放源码包。
- 包内不包含私钥、签发工具、客户资料、内部测试模型。
- 包内不包含本机绝对路径。
- 包名、版本号、适用系统清楚。
- SHA256 摘要已记录。
- 没有 license 时只能做有限检查，不能长期使用核心功能。
- Release 文案说明需要联系作者申请试用或付费 license。

## 文档

- 试用申请模板清楚。
- 联系方式正确。
- 隐私说明存在。
- 试用边界清楚。
- 不承诺自动修复所有模型。
- 不承诺保证收敛。
- 不暗示官方合作或官方认证。

## 演示图片和视频

- 使用公开示例、虚构模型或已脱敏案例。
- 隐藏路径、用户名、license 信息和客户信息。
- 不展示核心实现代码。
- 不展示完整客户模型。
- 不展示敏感几何、材料参数或项目名称。

## 社交平台

- 小红书、闲鱼、抖音、B站都导向 GitHub 页面或联系方式。
- 文案强调“先联系说明 Marc 版本和问题”。
- 不要求用户一开始发送完整模型文件。
- 不承诺免费长期使用。
- 不使用“官方”“破解”“免授权”等敏感或误导表达。

## 最终扫描

发布前扫描这些内容：

```text
.py .proc .ps1 .toml .json .mud .mfd .dat .t16 .t19 .out .sts .whl .exe
private key, license signing, customer, internal, absolute path, real project name
```

注意：闭源包可以作为 GitHub Release 资产发布，但不要提交进仓库目录和 git 历史。
