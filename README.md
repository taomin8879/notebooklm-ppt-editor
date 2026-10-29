# NotebookLM PPT Editor

**把图片型 PDF、PPTX 和幻灯片截图，重建为可编辑文字的 PowerPoint。**

[English](README.en.md) · [下载 Mac 测试版](https://github.com/taomin8879/notebooklm-ppt-editor/releases/download/v0.1.0-build186-public1/NotebookLM-PPT-Editor-0.1.0-build186-public1-macOS-arm64.dmg) · [安装说明](docs/INSTALL.zh-CN.md) · [结果检查指南](docs/QUALITY.md) · [反馈](https://github.com/taomin8879/notebooklm-ppt-editor/issues/new/choose)

> **0.1.0 · build 186 / public1 · 公开测试版**
>
> 仅支持 Apple 芯片 Mac（M 系列）、macOS 13+，需另装 LibreOffice。
>
> **尚未经过 Apple Developer ID 签名与公证**，首次打开可能被 macOS 阻止。请先阅读安装说明。

本项目是独立工具，与 Google / NotebookLM 无官方关联。本仓库提供完整桌面 App 的发布包和使用说明，不包含核心源码。

## 下载

| 文件 | 用途 |
| --- | --- |
| [完整 App 安装包（约 223 MB）](https://github.com/taomin8879/notebooklm-ppt-editor/releases/download/v0.1.0-build186-public1/NotebookLM-PPT-Editor-0.1.0-build186-public1-macOS-arm64.dmg) | 内含运行环境、OCR、背景修复模型和字体 |
| [SHA256SUMS.txt](https://github.com/taomin8879/notebooklm-ppt-editor/releases/download/v0.1.0-build186-public1/SHA256SUMS.txt) | 核对下载文件完整性 |
| [本次发布说明](https://github.com/taomin8879/notebooklm-ppt-editor/releases/tag/v0.1.0-build186-public1) | 验证范围、版本说明及限制 |

**普通用户不需要 Python、终端、API Key 或 AI Skill，也不需要首次下载模型。** LibreOffice 需要单独安装，用于渲染与质量核对。

## 能解决什么问题

| 输入或需求 | 输出与边界 |
| --- | --- |
| 图片型 PDF / PPTX 中的文字无法直接修改 | 将识别成功的文字重建为 PowerPoint 文本框 |
| 只有 PNG / JPG 幻灯片截图 | 按页面布局重建可编辑文字和图片层 |
| 希望保留复杂背景与装饰 | 复杂视觉区域可能保留为图片，不承诺全部图形可编辑 |
| 不确定转换结果是否可靠 | 查看“通过 / 可用但有提醒 / 需修正”和检查图，逐页复核 |

仅仅导出 `.pptx` 文件并不代表文字可以编辑。建议先用一页自制或获授权的材料试转，再在 PowerPoint 中实际选中文字修改。

## 三步试用

1. **安装。** 下载 DMG，把 App 拖到“应用程序”，另装 [LibreOffice](https://www.libreoffice.org/download/download-libreoffice/)。
2. **先试一页。** 拖入 PDF、PPTX、PNG 或 JPG/JPEG，选择页码和输出位置，使用默认本地模式。
3. **检查再使用。** 打开输出 PPTX 和检查图，核对漏字、错字、换行及遮挡；“需修正”不能视为验收通过。

完整步骤见 [安装与使用](docs/INSTALL.zh-CN.md)。不承诺 100% 还原、字体完全一致或所有元素都可编辑。

## 隐私与运行方式

- 默认本地模式，不需要 API Key；源文件不覆盖。
- DeepSeek 在线增强是可选项，启用前请确认材料可发送到配置的服务，可能产生 API 费用。
- 公开反馈只提交脱敏错误与自制样例，不要上传单位文件、客户资料或密钥。
- 可编辑覆盖率只针对识别出的文字，不保证没有漏识别；详见 [结果检查指南](docs/QUALITY.md)。

## 让 AI 助手调用（可选）

已经安装 App、希望通过本地 AI 助手批量调用时，再安装 [NotebookLM PPT Skill](https://github.com/taomin8879/notebooklm-ppt-skill)。Skill 有额外的 Python 与本地执行环境要求，普通桌面用户可以跳过。

## 反馈与授权

[提交安装或转换问题](https://github.com/taomin8879/notebooklm-ppt-editor/issues/new/choose)，请提供系统、芯片、版本、复现步骤和脱敏错误。涉及私人材料或授权咨询，请联系 [tommy_ai@126.com](mailto:tommy_ai@126.com)。

本仓库用于公开测试分发，不含支付或授权激活服务。主程序未授予开源许可；公开下载不等于获得源码或再分发权。第三方组件保留各自许可，随 App 提供 ThirdPartyNotices。没有 Windows、Intel Mac 或 Linux 安装包。
