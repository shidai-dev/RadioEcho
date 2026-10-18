# Radio Echo v0.1.13

日期 / Date: 2026-10-18

## 核心更新

- **USB 发射音频路由：** 修正 USB 接收收尾时恢复未由其修改的扬声器策略、复用发射音轨不刷新端点的问题；每轮重新匹配外部输出，检查实际路由并在断路时停止播放。另修正取消尚未装入音频的静态音轨时的清理异常。
- **电台状态回读：** 工作频率跟随真实回读，清除旧频点解码/目标，通联日志保留实际拨盘频率；DX10 新增 RM5/RM6 功率/驻波读取，CW 在驱动内采样以免界面查询阻塞在整段拍发之后。数值为公开标定点估算，不把设定功率当实际输出。
- **横屏 FT8 更紧凑：** 四个页面入口、通联摘要和呼叫/停止合并成单行底栏；保留 48dp 触控，接收/等待/发射不变高，减少大片红色状态区。竖屏不变，不改编解码、时隙、通联状态机或上传策略。

## Highlights

- Corrected USB input teardown policy ownership and stale TX endpoint reuse.
  External output is rebound per preparation; actual route changes stop PCM.
  Cancelling an unstaged static track no longer attempts an invalid pause.
- Operating frequency follows radio readback and completed logs retain the real
  dial. DX10 RM5/RM6 meter support uses approximate physical-scale estimates;
  CW-owned sampling/cache avoids UI queries behind a whole keyer operation.
- One landscape FT8 footer combines navigation, QSO summary and Call/Stop, keeps
  48dp touch targets and stable RX/WAIT/TX height. Portrait layout, codecs, UTC
  slot rules, QSO sequencing and upload policy are unchanged.

## Installation

Android 7.0+ / API 24; target API 35; `arm64-v8a` only.
Package: `cn.bi1rre.radioradioecho`; version: `0.1.13 (14)`.
Free Commercial preview, no activation, lightweight MIT-licensed `ft8_lib`.
Back up configuration and complete ADIF; cover-install the same-signature APK
without uninstalling. Download the independent APK, not GitHub's source archive.
See `INSTALL.md`, `RELEASE_MANIFEST.json` and `SHA256SUMS.txt` for final integrity data.

## Validation and Limitations

634 automated tests, TypeScript, native playback/decode/resampling and a
120-cycle/480-message receive soak passed. The 51 fixture-based component
checks included bilingual layouts, navigation and Stop. These do not replace
Android driver, native accessibility, USB hotplug, CW/FT8 continuous TX/RX or
physical power/SWR acceptance. The free Commercial APK uses formal BI1RRE
v2/v3 signing; package/version, arm64/JNI and TrustedQSL checks passed.

APK: `Radio-Echo-v0.1.13-android-arm64.apk` (34,533,671 bytes).
SHA-256: `e24253cd7abe63cfa10e9cce9b7aa0c06dfed68319a73a26e6f328d5e8f1d9b7`.

The fault log confirms speaker TX and an app-induced speaker-policy mutation,
but does not include the earliest AudioTrack creation. Do not interpret this
release as proof that every routing trigger is closed. DX10 scale estimates
need comparison against the radio and are not a calibrated safety instrument.

本版仍为 **Pre-release**。尚无本批修复后的真机验收结果；请由持证操作员在受控低功率环境下验证，保持物理停止手段。此前版本保留，不静默替换已发布 APK。

This remains a **Pre-release**. Keep a licensed operator present, test at low
power in a controlled setup, and retain a physical stop. Previous releases and
their APK bytes are retained unchanged.
