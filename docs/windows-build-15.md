# Windows 构建 15 · 2026-10-20

应用版本 **2.0.1+15**，适用于 **Windows 10 1809 / Windows 11 x64**。

- `CenYin-2.0.1+15-windows-x64-setup.exe`：安装版，默认安装到当前用户目录。
- `CenYin-2.0.1+15-windows-x64-portable.zip`：便携版，完整解压后运行 `CenYin.exe`，保留 `data/` 与全部 DLL。
- `SHA256SUMS-windows.txt`：两个成品包的 SHA-256 校验值。

安装版与便携版包含相同程序、播放器资源、媒体后端和 MSVC 可分发运行库。已有用户更新前可导出本地歌单备份。

## 本次桌面更新

- 播放页中的音质和播放器样式使用浮层；音质再次点击、点击外部或关闭按钮均可收起，不叠加弹窗。
- 音质偏好与实际播放档位分别保存，切歌按歌曲支持情况选择并回退，后续歌曲继续尝试原偏好档位。
- 底部封面与歌名再次点击可收起播放页，保留播放状态和进度。
- 青春彩胶按封面取色，固定样式保持各自配色，歌词统一灰白；调整唱针位置与底部控件，音质切换提示改为短时紧凑浮层。
- 右上角头像与昵称进入“我的”，提供资料修改；个性装扮入口集中在右上角，移除顶部重复小窗按钮。
- 今日心动默认每页四列、两行，支持鼠标或触控横向滑动和翻页，播放队列保留全部推荐歌曲。

## 下载

[安装版 EXE](https://github.com/cenguigui/CenYin-2.0/releases/download/v2.0.1-windows.15/CenYin-2.0.1%2B15-windows-x64-setup.exe) · [便携 ZIP](https://github.com/cenguigui/CenYin-2.0/releases/download/v2.0.1-windows.15/CenYin-2.0.1%2B15-windows-x64-portable.zip) · [校验文件](https://github.com/cenguigui/CenYin-2.0/releases/download/v2.0.1-windows.15/SHA256SUMS-windows.txt)

Windows 成品包同步发布在公开与私有 Releases；完整应用源码只保存于私有仓库。此前 Android APK、iOS IPA 与 Mac DMG 继续保留在对应版本的 Release，本次 Windows 发布不会改变它们的构建内容。

## 验证范围

Windows Release 已在本机构建和运行；桌面播放器、音质浮层、封面展开/收起、推荐横滑以及歌词配色的针对性组件测试通过，相关 Dart 文件静态分析通过。安装包另核对资源完整性与 SHA-256。Windows 系统媒体控制沿用 SMTC，迷你播放器为独立小窗；本次未实现嵌入任务栏的播放条。
