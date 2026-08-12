# Radio Echo v0.1.1 Android 公开预览版

本次更新集中改善 FT8 发射前的接收收尾、IC-705 WLAN 控制链路、CW 自动 CQ，以及日志与 LoTW 的日常操作体验。

## 核心变化

- FT8 只有在上一接收周期处理完成后才进入 PTT，减少发射抢占解码；
- IC-705 WLAN 分别监测控制、CI-V 和音频，重连时完整清理旧会话；
- CW 新增默认关闭的自动 CQ，并恢复两个国内 Spot 服务器预设；
- LoTW 同步迁移到日志页，新增默认关闭的 FT8 新通联自动上传选项；
- 页面按需加载，日志、地图、设置和窄屏 CW 的布局及响应速度得到调整。

## 下载文件

- `Radio-Echo-v0.1.1-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK SHA-256：

```text
f6d94ab5833b490cc90fffbc7825fec03085a66beea370b554184ab1ba987038
```

当前仅支持 Android `arm64-v8a`。FT8 自动流程与所有发射操作仍需持证操作员持续监督；LoTW 自动上传默认关闭，启用前请确认日志正确。完整限制和升级说明见 `RELEASE_NOTES_v0.1.1.md` 与 `INSTALL.md`。

建议将本 Release 标记为 **Pre-release**。
