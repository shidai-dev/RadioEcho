# Radio Echo v0.1.6

这是面向 Elecraft KX3 USB OTG 的维护版本，继续作为免费 Android `arm64-v8a` 公开预览版发布。

## 核心更新

- **KX3 连接：** KXUSB/FTDI 使用只读 CAT 回包确认连接，优先保留用户设置的速率，并依次尝试常见波特率，避免串口打开但电台不可控的假连接。
- **KX3 模式：** DATA A 使用 KX3 独立的 `MD6;DT0;` 映射，不再沿用通用 Kenwood 模式解释。
- **KX3 CW：** 使用官方等待式 `KYW` 命令按 24 字符分帧，收到 `KY0` 后再交付下一帧，最终以 `TQ0` 确认结束；不再轮询当前固件未可靠响应的 `TBX`。
- **音频边界：** KXUSB 仅承担 CAT。KX3 FT8 使用 `PHONES → Android 音频输入` 和 `Android 音频输出 → MIC` 的独立模拟音频链路。

## 已知限制

- KX3 的发送中取消、USB 热插拔恢复及 30 分钟连续运行仍需更多现场回归。
- FT8 音频效果取决于外置声卡、转接线、电平和 Android 音频路由；KXUSB 本身不提供音频。
- 当前仅提供 Android `arm64-v8a`，不提供 iOS、32 位或 x86 版本。

## 安装包

```text
文件：Radio-Echo-v0.1.6-android-arm64.apk
包名：cn.bi1rre.radioradioecho
版本：0.1.6 (7)
最低 Android：API 24
目标 Android：API 35
SHA-256：f947e1050058c23fddc536b3b909e9582eb1a5d8f7b2bb915b444df023c82102
签名证书 SHA-256：c2fad4dc5c79163f23fb80d97427c70f4a187be714546d890bf6ceea2bb819af
```

升级前建议导出配置和完整 ADIF。不要卸载旧版，使用同包名、同签名 APK 直接覆盖安装。本版本仍为 **Pre-release**，自动发射必须由具备相应资格的操作员持续监督。
