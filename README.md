# Concat 内置特效 - 简体中文汉化扩展

为 Concat 桌面版内置特效提供简体中文汉化，方便中文用户识别和使用特效及其参数。

本项目包含 **132 个汉化特效包**，汉化内容包括特效名称、分类、参数标签及说明。项目提供 Windows 和 Linux 平台的发行支持。

## 当前支持情况

| 项目 | 当前状态 |
|---|---|
| Concat 版本 | v0.2.11 |
| Windows | x86_64，已验证 |
| Linux | x86_64，已在 Linux Mint 22.3 验证 |
| 汉化语言 | 简体中文 |
| 特效包数量 | 132 |
| Linux 安装方式 | DEB 软件包 |

Linux 版已在 Linux Mint 22.3 x86_64 上验证，安装后可将 132 个特效部署到当前安装用户的 Concat 默认特效目录，并通过 Concat 软件内加载和使用测试。

Linux 发行目标为 Debian、Ubuntu 和 Linux Mint。目前实际验证的 Linux 发行版为 Linux Mint 22.3；Debian 和 Ubuntu 尚未完成实机验证。其他桌面平台及 Android 尚未完成验证。Concat 后续版本可能调整特效包格式或加载机制，不能据此推定未来版本始终兼容。

## 获取方式

请前往 [GitHub Releases](https://github.com/WenZoo1982/Concat-Chinese-Effects/releases) 下载发行版文件。

- **Windows x64**：提供安装程序和 ZIP 手动部署包。
- **Linux x86_64**：提供 DEB 安装包。

## Linux 安装

下载 `concat-chinese-effects-1.0.0-Linux-x86-64.deb` 后，在下载目录打开终端，执行：

```bash
sudo apt install ./concat-chinese-effects-1.0.0-Linux-x86-64.deb
```

如果已经安装过相同版本，需要重新安装时，执行：

```bash
sudo apt install --reinstall ./concat-chinese-effects-1.0.0-Linux-x86-64.deb
```

安装程序会识别当前安装用户，并将汉化特效部署到该用户的 Concat 默认特效目录：

```text
~/.config/app.concat.editor/effects/
```

例如，用户 `wenzoo` 的安装位置为：

```text
/home/wenzoo/.config/app.concat.editor/effects/
```

安装时，同名文件会被覆盖更新，目标目录中的其他文件会保留。卸载 DEB 软件包不会自动删除用户目录中的特效文件。

安装完成后，在 Concat 中刷新或重新打开特效页面即可使用。

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

A Simplified Chinese localization for Concat's built-in effects. This project includes 132 localized effect packages and supports Windows x86_64 and Linux x86_64. It has been tested with Concat v0.2.11 on Windows and Linux Mint 22.3.

The Linux DEB package installs the effects into the current installing user's default Concat effects directory:

`~/.config/app.concat.editor/effects/`

Files with matching names are overwritten during installation, while other files in the destination directory are preserved. Uninstalling the DEB package does not automatically remove the user's effects files.

The Linux DEB package is available on the [GitHub Releases page](https://github.com/WenZoo1982/Concat-Chinese-Effects/releases).
