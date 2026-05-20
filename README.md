# RioConfig

[Rio Terminal](https://rioterm.com/) 终端配置文件，支持中文和 Emoji 显示。

## 字体配置

- **西文字体**：Cascadia Code（Rio 默认字体）
- **中文字体**：[Sarasa Term SC](https://github.com/be5invis/Sarasa-Gothic)（更纱黑体等宽终端版 - 简体中文）
- **Emoji 字体**：Segoe UI Emoji（Windows 系统自带）

### 安装更纱黑体

从 [Sarasa Gothic Releases](https://github.com/be5invis/Sarasa-Gothic/releases) 下载 **Term** 包（如 `SarasaTerm-TTF-Unhinted-x.x.xx.7z`），解压后安装其中带 `SC` 的 TTF 文件即可。

## 配置文件路径

| 平台 | 路径 |
|------|------|
| Windows | `%USERPROFILE%\AppData\Local\rio\config.toml` 或 `$env:USERPROFILE\AppData\Local\rio\config.toml`（PowerShell） |
| Linux | `$XDG_CONFIG_HOME/rio/config.toml` 或 `~/.config/rio/config.toml` |
| macOS | `~/.config/rio/config.toml` |

也可以通过设置 `$RIO_CONFIG_HOME` 环境变量来自定义配置路径，它会替代 `~/.config/rio` 来读取配置、主题等文件。

配置文件修改后会自动触发 Rio 重新渲染，无需手动重启。

## 使用方法

将 `config.toml` 复制到对应平台的 Rio 配置路径下即可。