# 构建 15 · 桌面、平板与续播

2026-10-19 · 应用版本 2.0.1+15。

- 桌面左侧导航、统一顶部搜索/返回、底部播放控制；歌单、榜单、搜索为宽屏歌曲表格，播放页采用左唱片、右歌词。
- 宽屏平板自动切换桌面布局；窄屏/竖屏恢复手机布局，保留搜索与页面状态。
- 鼠标/触控板浏览歌词时提供选择线和播放按钮，可定位当前歌词；全部平台点击封面暂停/继续。桌面隐藏滚动条，进度和音量条统一细线样式。
- 关闭后保留队列、歌曲、进度和播放状态。重新打开时先获取新的在线 URL，再恢复进度；暂停的歌曲继续保持暂停，本地歌曲读取文件。
- iOS/macOS 增加 10 段原生均衡器，继续使用原后台播放与媒体会话。本地与 MP3/FLAC 在线文件适用；HLS 直播不适用。Windows 当前后端尚未接入均衡器。
- 蛋仔与林俊杰背景装饰跟随歌曲圆心，光遇重新截图复核；[三款播放/暂停原图](screenshots/ios-style-alignment/README.md)。
- 保留 iOS 下载 FLAC、歌词、皮肤、统一手势、队列居中和定位修复。旧版已损坏的 FLAC 文件仍需重新下载一次。

## 安装包

[发布与下载](https://github.com/cenguigui/CenYin-2.0/releases/tag/v2.0.1-desktop.15)

- iOS：`CenYin-2.0.1+15-ios-arm64-unsigned.ipa`，iOS 15 及以上，真机 Release，需自行签名。
- Mac：`CenYin-2.0.1+15-macos-universal.dmg`，macOS 12 及以上，Apple silicon/Intel，测试临时签名，未通过 Developer ID 公证。
- Windows：已补充[安装版 EXE、便携 ZIP 与校验值](https://github.com/cenguigui/CenYin-2.0/releases/tag/v2.0.1-windows.15)，Windows 10 1809 / Windows 11 x64；[本机更新与验证](windows-build-15.md)。

实测包括 Mac 原生在线/下载 MP3、FLAC、暂停/继续/进度跳转；Mac 与独立 iOS 模拟器原生均衡器输出和 37 秒暂停恢复；Mac 完全关闭后 30 首队列及 1:42 进度自动恢复。组件测试不代表 Android 真机帧率或 Windows 系统媒体控件实机验收。

[桌面截图](screenshots/desktop/README.md) · [完整 19 款播放器图库](screenshots/ios-player-styles/README.md)
