# GitHub 仓库设置建议

这些设置需要在 GitHub 网页端手动完成。

## About

Repository description 建议填写：

```text
Windows closed-source AI workflow assistant for MSC Marc/Mentat users.
```

Website 可以先留空，后续如果有主页、视频或文档站再填。

Topics 建议：

```text
msc-marc
mentat
marc
mcp
codex
finite-element-analysis
fea
solver-diagnosis
post-processing
windows
```

## Issues

建议暂时保留 Issues，但不要把 Issues 当作主要支持渠道。

原因：

- 公开 Issue 有利于展示有人关注；
- 可以承接一般问题；
- 但用户不应该在 Issue 里上传模型、日志和敏感资料。

仓库已提供 Issue 模板，用于提醒用户不要公开完整模型文件和敏感信息。

## Releases

当前先不要上传闭源包。

等第一位灰度用户测试通过后，再考虑创建 Release，例如：

```text
v2.5.0-trial
```

Release 描述应明确：

- Windows only；
- closed-source package；
- requires local license；
- no Marc/Mentat software included；
- no Marc/Mentat license included；
- contact author for trial/pro license。

## License

当前不建议添加开源 license。

不添加 license 的含义是：公开仓库里的文字和材料可以被浏览，但不等于授权他人复制、改造或商用核心内容。后续如果需要，可以单独写一个更明确的 All rights reserved 声明。
