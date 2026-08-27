# Radio Echo v0.1.4 Android 公开预览版

本次更新以设备控制和发射稳定性为主，不扩大未经真机验证的兼容性声明。

## 核心变化

- FT-DX10 USB CW 改用 Standard 串口 DTR 键控，已完成快捷语真机拍发验证；
- FX-4CR 蓝牙无 CAT 回包时自动进入“仅控制”模式，避免状态与 PWR/SWR 查询持续超时；
- 改进 FT8 自动续发门禁、定向 CQ/六位网格识别和不同连接方式的 PTT 时序；
- 保持 FT8、CW、日志与具体设备驱动分层，新增兼容处理不进入业务页面。

## 下载文件

- `Radio-Echo-v0.1.4-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK SHA-256：

```text
e4a322f95eb316a1bff8f2ffe283fda1f71670cc0a0560557946a823ae24d7ff
```

当前仅支持 Android `arm64-v8a`。FX-4CR USB 回读与表计、IC-705 USB FT8 连续发射、通用 USB 音频以及未持有真机的 USB 电台目录仍属于实验性能力。所有发射操作必须由持证操作员持续监督。

建议将本 Release 标记为 **Pre-release**。
