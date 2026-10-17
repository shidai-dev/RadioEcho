# Radio Echo v0.1.11

日期 / Date: 2026-10-17

## 核心更新

1. **FT8 定向应答：** 自动 CQ 时优先处理明确呼叫本台的有效消息；关闭自动找台不再关闭定向应答。已通应答仍遵循设置，纯接收不会自动发射。
2. **发射与等待：** 将接收准备和界面通知移出临近发射的关键路径；Android 整帧音频提前准备并由原生时钟调度，完善停止与接收恢复。排队显示实际 UTC 和剩余秒数，保留真正迟到跳过，不靠增加延迟掩盖问题。
3. **横屏工作台：** 频谱在左、解码与控制在右，列表独立滚动，主要操作保持可达，避免频谱挤走解码信息。

## Highlights

- Prioritize valid calls addressed to your station during automatic CQ. Directed
  replies remain available when target hunting is disabled, subject to settings;
  passive reception never starts transmission.
- Move receive preparation and UI notifications out of the transmit-start
  critical path. Pre-stage complete Android audio frames with native scheduling,
  cancellation and receive recovery; show actual queued UTC and countdown.
  Genuine late starts are still skipped, without extending timing limits.
- Place the spectrum beside decodes in landscape, with independently scrolling
  results and accessible QSO controls.

## Build and Upgrade

Android 7.0+ / API 24, target API 35, `arm64-v8a`.
Package: `cn.bi1rre.radioradioecho`; version: `0.1.11 (12)`.
Free Commercial preview, no activation, lightweight MIT-licensed `ft8_lib`.
Download the independent APK asset, not GitHub's document source archive.
Export configuration and full ADIF first, then upgrade without uninstalling.
See `INSTALL.md`, `SHA256SUMS.txt` and `RELEASE_MANIFEST.json`.

## Validation and Limitations

- TypeScript, 595 automated tests, native playback/snapshot helper tests,
  encode/decode, PCM resampling and host receive soak (120 cycles / 480 valid
  messages) passed. Commercial Release and formal BI1RRE v2/v3 signatures passed.

本次修改已通过自动化和构建检查，尚未完成新版真机界面、音频路由及射频通联验收，不能视为现场问题已全部解决。请先低功率受控测试，保持操作员监督和物理停止手段。

This is a **Pre-release**. Automated tests, native helper tests and host receive
soak do not replace hardware acceptance. The new native AudioTrack route,
continuous automatic QSOs, actual PTT/audio timing, output power, cancellation,
RX recovery and Chinese/English landscape/keyboard behavior still require
device and on-air verification. Radio-specific CAT commands and codec algorithms
are unchanged. Keep a licensed operator present and a physical emergency stop
available. Previous releases remain available for comparison.
