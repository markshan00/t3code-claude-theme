# Claude Desktop：T3 Code 配色主题

[English](README.md)

将 Claude 桌面的暖白底色、炭灰深色和陶土色强调色带到 [T3 Code](https://github.com/pingdotgg/t3code)。一个原生主题 JSON 文件，同时包含浅色和深色配色。

![浅色与深色配色预览](assets/preview.svg)

*预览为使用真实主题颜色绘制的示意界面，并非应用截图。*

## 安装

1. [下载 claude-desktop.json](https://github.com/markshan00/t3code-claude-theme/releases/latest/download/claude-desktop.json)。
2. 在 T3 Code 中打开 **设置 → 外观 → 导入主题**。部分版本会将主题分组显示为 **颜色与主题**。
3. 选择下载的 JSON 文件，或者将文件内容粘贴到主题导入框，确认导入。
4. 选择 **Claude Desktop**，分别将其浅色、深色预览设为对应模式使用的主题；需要跟随系统切换时，选择 **系统** 外观。

也可以[查看并复制原始 JSON](https://raw.githubusercontent.com/markshan00/t3code-claude-theme/main/claude-desktop.json)。无需安装扩展、编译或执行脚本。主题操作可参考 T3 的[官方外观说明](https://github.com/pingdotgg/t3code/blob/main/docs/user/appearance.md)。

## 配色

| 用途 | 浅色 | 深色 |
| --- | --- | --- |
| 主背景 | `#fcfcfb` | `#151515` |
| 侧栏 | `#fcfcfb` | `#111111` |
| 正文 | `#0b0b0b` | `#f0efec` |
| 次级文字 | `#52514e` | `#c3c2b7` |
| 强调色 | `#c6613f` | `#c6613f` |

每套配色定义 57 个颜色项，覆盖对话、侧栏、工具栏、代码块、终端和状态提示。主题只改变颜色，不包含 Claude 字体，也不改变 T3 布局。

采用 T3 version 1 主题格式，固定 ID 为 `claude-desktop`。如果已经安装同 ID 主题并做过修改，覆盖前先导出自己的版本。

## 来源与兼容性

主题于 2026 年 10 月 4 日根据 Claude 桌面缓存中的设计 token 和桌面框架样式制作。发布配色与维护者正在使用的「Claude 桌面」一致；仅将显示名称改为 **Claude Desktop**，方便分享。详见[来源与验证记录](docs/provenance.md)。

由 [Mark](https://github.com/markshan00) 维护。这是非官方社区主题，与 Anthropic、T3 Tools 无隶属或背书关系；产品名称归各自权利人所有。

本主题适配、文档和预览图采用 [MIT 许可证](LICENSE)，不包含第三方产品原始素材。
