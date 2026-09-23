# Radio Echo v0.1.6 Android 公开预览版

本次维护版本新增 Elecraft KX3 USB OTG 基础支持，并修复 KX3 CAT CW 长报文只拍发少量字符的问题。

## 核心变化

- KXUSB/FTDI 连接按用户设置优先，自动只读探测 `38400/19200/9600/4800`；
- KX3 DATA A 使用独立 CAT 模式映射，频率和模式控制已完成基础真机验证；
- CW 改用 KX3 官方等待式 `KYW` 队列，长快捷语按 24 字符安全分帧并等待电台确认完成；
- 明确 KXUSB 只提供 CAT，FT8 必须使用 KX3 `PHONES` 与 `MIC` 的独立模拟音频链路。

## 下载文件

- `Radio-Echo-v0.1.6-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK SHA-256：

```text
f947e1050058c23fddc536b3b909e9582eb1a5d8f7b2bb915b444df023c82102
```

当前仅支持 Android `arm64-v8a`。KX3 发送中取消、USB 热插拔恢复和长时间运行仍需更多现场样本；所有发射操作必须由持证操作员持续监督。

本 Release 标记为 **Pre-release**。
