# Radio Echo v0.1.10 Android 公开预览版

## 核心更新

- 重整 CW/FT8 户外工作台，改善横屏调频、固定操作区和解码语义配色。
- 精简日志、查询和设置，突出新增/LoTW 同步，保存失败保留草稿，补齐中英文提示。
- 修复 FT8 有采样却显示等待音频、空扫描状态及切源/切频后的旧状态残留。

## Highlights

- Cleaner CW/FT8 field workspaces, improved landscape tuning and classic decode colors.
- Simpler logging, queries and settings, retained drafts on save failure and clearer bilingual feedback.
- Correct native FT8 receive status for live samples, empty scans and source/frequency changes.

免费预览，无需授权码。Android 7.0+，仅 `arm64-v8a`，正式签名，可保留数据覆盖升级，建议先备份配置和 ADIF。

This free preview uses the lightweight `ft8_lib` backend. Radio protocols and QSO timing are unchanged. Dense-signal decoding, continuous automatic QSOs and live TX/RX recovery still require field acceptance; this is not a desktop WSJT-X/JTDX equivalent. 发射必须由持证操作员监督。

独立 APK、`SHA256SUMS.txt` 和 `THIRD_PARTY_NOTICES.md` 见附件。此版本为 **Pre-release**。
