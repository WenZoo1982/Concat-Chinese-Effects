# Concat 内置特效 - 汉化扩展

为 Concat 桌面版内置特效提供简体中文汉化，方便中文用户识别和使用特效及其参数。

本项目目前包含 **132 个汉化特效包**，汉化内容包括特效名称、分类、参数标签及说明。

## 当前支持情况

| 项目 | 当前状态 |
|---|---|
| Concat 版本 | v0.2.10 |
| 已验证平台 | Windows x86_64 |
| 汉化语言 | 简体中文 |
| 特效包数量 | 132 |
| 验证情况 | 已在上述环境中加载并实际使用 |

目前仅将 Windows x86_64 列为已验证平台。其他桌面平台及 Android 尚未完成验证。Concat 后续版本可能调整特效包格式或加载机制，不能据此推定未来版本始终兼容。

## 获取方式

项目提供以下两种 Windows x64 分发版本：

- **安装版**：使用安装程序部署汉化特效包。
- **ZIP 手动部署版**：下载压缩包，手动解压并复制特效包文件。

请前往 [GitHub Releases](https://github.com/WenZoo1982/Concat-Chinese-Effects/releases) 下载发行版文件。

## 项目来源与修改范围

- 上游项目：[Concat](https://github.com/jub0t/Concat)
- 上游特效包来源：Concat 仓库中的内置特效包。
- 本项目包含 132 个汉化特效包。
- 汉化修改集中在特效包清单文件 `effect.toml`，包括第三方特效包 ID、显示名称、分类、参数标签及说明等界面文本。
- 特效着色器及其他非清单资源文件保持上游原样，未作修改。

本项目是由社区维护的第三方汉化扩展，与 Concat 原作者及官方项目没有隶属或背书关系。Concat 名称及相关商标仍归其权利人所有。

## 许可证

本项目中基于 Concat 内置特效包修改和再分发的内容，按上游项目适用的 **GNU Affero General Public License v3.0 or later（AGPL-3.0-or-later）** 发布。完整许可证文本见仓库根目录的 [LICENSE](LICENSE)。

原始作品的版权归原作者及相应权利人所有。汉化修改不意味着取得原始作品的独立所有权。更多来源、版权及修改说明见 [NOTICE.md](NOTICE.md)。

AGPL 允许使用、修改和再分发，但再分发时必须遵守许可证要求；不得通过附加限制剥夺接收者在该许可证下享有的权利。

---

**English**

A Simplified Chinese localization for Concat's built-in effects. This project includes 132 localized effect packages and has been tested with Concat v0.2.10 on Windows x86_64.

Windows x64 installer and manual ZIP distribution are available on the [GitHub Releases page](https://github.com/WenZoo1982/Concat-Chinese-Effects/releases).
