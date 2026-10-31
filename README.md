# T2I Studio · 发布页

T2I Studio 桌面版（二次元二创文生图提示词速构台）的**安装包下载与更新日志**仓库。源码私有，这里只放打包产物。

## 下载与升级

到 [Releases](https://github.com/ShaLuuFPS/t2i-studio-releases/releases) 下载最新的 `T2I Studio_x.y.z_x64-setup.exe`，双击安装。

**覆盖安装即升级**：词库 / 参数 / 工作流都存在本地数据目录，不会被清掉，也不需要卸载旧版。

- 系统要求：Windows 10 / 11 x64（WebView2 运行时；Win11 自带，Win10 若提示缺失装一下即可）
- 安装包没有代码签名证书，SmartScreen 提示「未知发布者」时点「更多信息 → 仍要运行」
- 应用内点顶栏版本号可「检查更新」，读取的就是本仓库的最新版本号

## 数据位置

| 内容 | 路径 |
| --- | --- |
| 默认提示词配置 | `%APPDATA%\com.t2i-autoprompt.desktop\default-prompts.json` |
| 词库勾选 / 生图参数 / 工作流（WebView2 localStorage） | `%LOCALAPPDATA%\com.t2i-autoprompt.desktop\EBWebView\Default\Local Storage\leveldb\` |

卸载不会删除这些数据；想彻底清干净再手动删这两个目录。

## 许可与数据来源

随包手册有完整说明。标签数据来源 BooruTagCart（GPL-3.0）与 EhTagTranslation（CC BY-NC-SA 3.0），本软件免费分发、仅供个人非商业使用；应用不含遥测，不向外发送任何使用数据。