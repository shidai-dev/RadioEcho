# Radio Echo v0.1.15 Android 公开预览版

## 核心更新 / Highlights

- **手机日志布局：** 横屏合并查询与操作工具栏，竖屏整合视图选择与搜索，减少上下固定栏占高，让日志正文显示更多记录。窗口变化保留搜索，表单适应短窗口；电台、音频、FT8 和上传策略不变。
- **More room for logs on phones:** compact landscape tools, combined portrait view/search controls, less fixed-bar padding and shorter-window forms. Search survives resizing; radio, audio, FT8 and upload behavior are unchanged.

## 验证与限制 / Validation And Limitations

709 automated tests, TypeScript, 18 bilingual log component cases, 16 shared
navigation/stop cases and signed release APK checks passed.
**手机原生输入法/系统栏与大字体仍待验收；长时间接收的高内存问题仍在调查，尚未修复。**
**Native phone acceptance remains pending; excessive memory during extended receive remains unresolved.**

免费、无需授权码；Android 7.0+，仅 arm64-v8a，轻量 ft8_lib 后端，版本 `0.1.15 (16)`。仍为 **Pre-release**。升级前备份配置和完整 ADIF，覆盖安装同签名 APK；不卸载、不清除数据。

Download the independent APK below, not GitHub's source archive. Back up full
configuration and ADIF before upgrading. Keep operator supervision and a
physical stop available. Previous release assets remain unchanged.
