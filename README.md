# Concat 中文特效扩展

Concat 内置特效的汉化扩展。Chinese localization for Concat built-in effects.

本项目为 Concat 桌面版提供中文特效包，将部分内置特效的界面名称、参数标签、分类及说明翻译为简体中文，方便中文用户识别和使用。

## 当前支持情况

| 项目 | 当前状态 |
|---|---|
| Concat 版本 | v0.2.10 |
| 已验证平台 | Windows x86_64 |
| 汉化语言 | 简体中文 |
| 特效包数量 | 132 |
| 验证情况 | 已在上述环境中加载并实际使用 |

目前仅将 Windows x86_64 列为已验证平台。其他桌面平台及 Android 尚未完成验证。Concat 后续版本可能调整特效包格式或加载机制，不能据此推定未来版本始终兼容。

## 安装方法

1. 关闭 Concat。
2. 下载本仓库，并解压到本地。
3. 打开 Windows 文件资源管理器，在地址栏输入以下路径：

   `%APPDATA%\app.concat.editor\effects`

   对应的完整路径通常为：

   `C:\Users\<用户名>\AppData\Roaming\app.concat.editor\effects`

4. 如果目标位置没有 `effects` 文件夹，请自行创建。
5. 打开解压后的项目目录，进入仓库中的 `effects` 文件夹。
6. 将 `effects` 文件夹内的 132 个 `wenzoo.*-cn` 特效包文件夹，直接复制到 Concat 用户目录下的 `effects` 文件夹中。
7. 重新启动 Concat。

**重要：复制的是仓库 `effects` 目录里面的 132 个特效包文件夹，不是把仓库整个 `effects` 文件夹或项目根目录复制进去。** 不要在目标目录中额外套一层总文件夹。

正确的仓库结构：

```text
Concat-Chinese-Effects/
├── LICENSE
├── NOTICE.md
├── README.md
└── effects/
    ├── wenzoo.glow-cn/
    │   └── effect.toml
    ├── wenzoo.posterize-cn/
    │   └── effect.toml
    └── ...（共 132 个特效包）
```

正确的 Concat 用户特效目录结构：

```text
%APPDATA%\app.concat.editor\effects/
├── wenzoo.glow-cn/
│   └── effect.toml
├── wenzoo.posterize-cn/
│   └── effect.toml
└── ...（共 132 个特效包）
```

Concat 会扫描 `effects` 目录的直接子文件夹。若额外套一层目录，特效包将无法按预期被发现。

## 卸载方法

关闭 Concat，然后从 Concat 用户目录的 `effects` 文件夹中删除本项目添加的 `wenzoo.*-cn` 文件夹即可。请勿删除其他来源的特效文件夹，也不要直接删除整个 `effects` 文件夹。

## 项目来源与修改范围

- 上游项目：[Concat](https://github.com/jub0t/Concat)
- 上游特效包来源：Concat 仓库中的内置特效包。
- 本项目包含 132 个汉化特效包。
- 汉化修改集中在特效包清单文件 effect.toml，包括第三方特效包 ID、显示名称、分类、参数标签及说明等界面文本。
- 特效着色器及其他非清单资源文件保持上游原样，未作修改。

本项目是由社区维护的第三方汉化扩展，与 Concat 原作者及官方项目没有隶属或背书关系。Concat 名称及相关商标仍归其权利人所有。

## 许可证

本项目中基于 Concat 内置特效包修改和再分发的内容，按上游项目适用的 **GNU Affero General Public License v3.0 or later（AGPL-3.0-or-later）** 发布。完整许可证文本见仓库根目录的 [LICENSE](LICENSE)。

原始作品的版权归原作者及相应权利人所有。汉化修改不意味着取得原始作品的独立所有权。更多来源、版权及修改说明见 [NOTICE.md](NOTICE.md)。

AGPL 允许使用、修改和再分发，但再分发时必须遵守许可证要求；不得通过附加限制剥夺接收者在该许可证下享有的权利。

---

**English**

A Simplified Chinese localization extension for Concat's built-in effects. It currently contains 132 localized effect packages and has been tested with Concat v0.2.10 on Windows x86_64.

See the sections above for installation instructions, compatibility notes, project provenance, and licensing.
