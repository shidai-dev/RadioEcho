# Radio Echo v0.1.10

日期 / Date: 2026-10-16

## 核心更新

1. **户外工作台：** CW 横屏采用有界双栏，频率、快捷语、日志与查询分区更清楚；精细调谐不再与快捷频率挤压。FT8 解码与通联控制独立滚动，主操作固定，采用 CQ、新台、已通和呼叫本台的经典语义配色。
2. **查询与管理：** 日志突出新增/LoTW 同步，导入导出集中到更多菜单；保存等待真实结果，失败保留草稿并可重试。传播筛选、错误恢复和设置更简洁，改善窄屏日期、中英文同步及接收提示。
3. **接收状态：** 修复原生 FT8 采样正常却提示等待音频，区分空扫描与断流，切源、切频及收发边界清理旧显示状态；没有改动电台协议、编解码算法或通联时序。

## Highlights

- Reorganized CW/FT8 field workspaces, improved landscape tuning, independent decode/control scrolling and classic decode colors.
- Simpler logs, propagation queries and settings; save failures retain drafts, with clearer retry and bilingual feedback.
- Native FT8 receive status follows current-session samples and decode completion instead of stale fallback state.

## Build and Upgrade

Android 7.0+ / API 24, target API 35, `arm64-v8a`.
Package: `cn.bi1rre.radioradioecho`; version: `0.1.10 (11)`.
Free Commercial preview, no activation, lightweight MIT-licensed `ft8_lib` backend.
Use the same-signature APK to upgrade without uninstalling; export configuration
and full ADIF first. Download the independent APK asset, not GitHub's document
source archive. Integrity and signing information: `SHA256SUMS.txt`,
`RELEASE_MANIFEST.json` and `INSTALL.md`.

## Validation and Limitations

- TypeScript, 567 automated tests and host FT8 soak (120 cycles / 480 valid messages) passed before version packaging; final packaging checks are recorded in the release manifest and internal checklist.
- CW/FT8, logs, settings, Chinese/English, tablet rotation, keyboard access and microphone status were checked on Lenovo TB324ZC. No new end-to-end RF or LoTW submission acceptance is claimed.
- Dense multi-signal reception, continuous automatic QSOs, actual TX/RX recovery, file-picker/network-failure paths and all radio/firmware combinations remain field-test areas. Simulated states and environmental microphone noise do not replace these tests.
- Keep the licensed operator present and a physical emergency stop available. This is a **Pre-release**; the previous Release remains available for comparison.
