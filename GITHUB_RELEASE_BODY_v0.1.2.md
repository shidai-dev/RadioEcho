# Radio Echo v0.1.2 Android 公开预览版

本次更新集中改善 CW、FT8、日志、传播和设置工作区的界面层级，并增加 FT8 定向 CQ、呼号输入修复和更完整的现场诊断信息。

## 核心变化

- 统一 Material 3 视觉层级、响应式断点、触控尺寸和状态反馈；
- FT8 解码区更宽，主通联操作更靠前，断开态去除重复麦克风入口；
- 新增 `CQ DX`、洲、USA、POTA、SOTA、TEST 和自定义定向 CQ；
- 修复英文输入法下呼号与网格重复追加字符；
- 日志、DXCC 与传播结果采用更紧凑的响应式布局和分批展示；
- 增强 FT8 周期完整性、候选过滤和发射后恢复诊断。

## 下载文件

- `Radio-Echo-v0.1.2-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK SHA-256：

```text
84eb47c3f5e119de39e079780d81da564f8b03a0a99a428ec12e7a419c735ade
```

当前仅支持 Android `arm64-v8a`。FT8 自动流程与所有发射操作仍需持证操作员持续监督；LoTW 自动上传默认关闭，启用前请确认日志正确。完整限制和升级说明见 `RELEASE_NOTES_v0.1.2.md` 与 `INSTALL.md`。

建议将本 Release 标记为 **Pre-release**。
