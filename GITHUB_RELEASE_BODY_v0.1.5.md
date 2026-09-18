# Radio Echo v0.1.5 Android 公开预览版

本次更新重点改善户外操作界面、Android 表单输入稳定性，并恢复 FX-4CR 修复版蓝牙固件的双向 CAT 与 PWR/SWR 表计。

## 核心变化

- 重构户外工作台、底部导航、全局发射停止入口和无线电语义配色；
- 修复日志表单滑动闪烁、CW 字段高度及呼号/信号报告输入；
- FX-4CR 修复版蓝牙固件恢复频率、模式、PTT、PWR 和 SWR 回读，旧固件仍可安全降级；
- FT8 音频和解码生命周期只归属 FT8 工作区，降低对 CW 与其他页面的影响。

## 下载文件

- `Radio-Echo-v0.1.5-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK SHA-256：

```text
0e631cfdd7796ddafaebb65950ef0cf7b0e998c0b76510de0247c4e4dbe11610
```

当前仅支持 Android `arm64-v8a`。实验性 USB 电台、不同固件和音频路由仍需更多真机验证；所有发射操作必须由持证操作员持续监督。

本 Release 标记为 **Pre-release**。
