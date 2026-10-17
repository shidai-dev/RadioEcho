# Radio Echo v0.1.11 Android 公开预览版

## 核心更新

- FT8 自动 CQ 优先应答本台定向呼叫，修正关闭找台后无法应答的问题。
- 调整发射准备与原生音频调度，减少错过时隙后反复等待；完善取消及接收恢复，显示实际 UTC 排队倒计时。
- FT8 横屏采用左频谱、右解码/控制布局，避免解码信息被挤出视野。

## Highlights

- Prioritize valid directed replies during automatic CQ, independently of target hunting.
- Improve transmit preparation and native audio scheduling, cancellation, RX recovery and queued-slot feedback without extending timing limits.
- Side-by-side spectrum and decodes in landscape, with accessible QSO controls.

免费预览，无需授权码。Android 7.0+，仅 `arm64-v8a`，正式签名，可保留数据覆盖升级；请先备份配置和 ADIF。

**仍需真机与射频复测：** 本次自动化通过不代表新版音频路由、持续通联及界面已完成现场验收，请在低功率受控环境中测试。发射必须由持证操作员监督。

This free preview uses the lightweight `ft8_lib` backend. Native AudioTrack routing, continuous QSOs and live TX/RX recovery still require hardware acceptance; automated tests are not on-air validation. Radio-specific CAT commands and codec algorithms are unchanged.

独立 APK、`SHA256SUMS.txt`、`THIRD_PARTY_NOTICES.md` 及双语版本说明见附件。此版本为 **Pre-release**。
