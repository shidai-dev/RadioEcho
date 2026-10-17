# Radio Echo v0.1.12

日期 / Date: 2026-10-18

## 核心更新

- **通联工作台更清楚：** 精简重复状态栏，固定 CW 保存/停止与 FT8 通联操作；横屏给频谱和解码留出更多空间，自动通联接收间隙及跨页/弹窗也保留停止。
- **日志管理更方便：** 新增、同步、搜索入口固定，筛选和完整同步/错误详情按需打开；地图合并重复标题，切换视图回到结果顶部。
- **查询与设置更整洁：** 传播筛选使用有界弹窗，设置减少重复分组，优化证书与密码操作及中英文可读性。设备协议、音频、编解码、通联状态机和上传策略不变。

## Highlights

- Cleaner CW/FT8 workspaces, fixed save/stop controls and more landscape space
  for spectrum and decodes. Stop remains available during automatic receive
  gaps, across tabs and in dialogs.
- Fixed log commands/search, on-demand filters and complete sync/error details;
  map view tools are consolidated and view changes return to the result top.
- Bounded propagation filters, simpler settings, improved certificate/password
  controls and bilingual readability. Radio protocols, audio, codecs, QSO
  sequencing and upload policy remain unchanged.

## Installation

Android 7.0+ / API 24; target API 35; `arm64-v8a` only.
Package: `cn.bi1rre.radioradioecho`; version: `0.1.12 (13)`.
Free Commercial preview, no activation, lightweight MIT-licensed `ft8_lib`.
Export configuration and full ADIF first; upgrade with the same-signature APK
without uninstalling. Download the independent APK, not GitHub's source archive.
See `INSTALL.md`, `RELEASE_MANIFEST.json` and `SHA256SUMS.txt`.

## Validation and Limitations

614 automated tests, TypeScript and 49 Chinese/English component-layout and
interaction scenarios passed. These previews used fixture data, a simulated
spectrum and the offline map renderer, not Android screenshots or RF signals.
The free Commercial APK is formally signed by BI1RRE (v2/v3).

APK: `Radio-Echo-v0.1.12-android-arm64.apk` (34,517,280 bytes).
SHA-256: `054236a97d3899adc0fd65124a6b0b6ee30ae1181d93eda15b3d6676026c67c1`.

本版仍为 **Pre-release**。Android 真机横屏、键盘/大字体、原生频谱及持续射频收发验收尚未完成；上一版本原生音频路由和持续自动通联的现场验收也未因此完成。请低功率受控测试，保持持证操作员监督和物理停止手段。

Android rotation, keyboard/large fonts, native spectrum and supervised continuous
TX/RX still need device acceptance. Earlier native audio-routing and continuous
automatic QSO field acceptance also remain pending. Keep a licensed operator
present and a physical emergency stop available. Previous releases remain intact.
