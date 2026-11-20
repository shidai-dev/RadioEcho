# Radio Echo v0.1.19

2026-11-20 · Public preview / 公开预览版 · Android 7.0+ · ARM64

## 更新内容

- **呼号通联历史自动查询**：在 CW / 语音中输入对方呼号，自动汇总本地与已缓存 LoTW 的通联次数；点击历史入口查看以往的波段、模式、UTC 时间和频率，不消耗 QRZ 查询配额。
- 改善大量日志的加载，修复日志搜索时列表变化导致的闪退。

## Highlights

- **Automatic callsign history:** Enter a DX callsign in CW / Voice to see QSO counts from local logs and cached LoTW history. Open history to review previous bands, modes, UTC times and frequencies without using QRZ queries.
- Improved loading of large logs and fixed a crash caused by list changes during log searches.

## 使用范围 / Preview Limits

本版包含仍在进行的 Java 迁移。CW 实时输入的连续性与停止、IC-705 语音、部分电台连接、真实 LoTW 签名上传与恢复、手机布局及完整中英文横竖屏验收尚未全部完成。大量 LoTW 自动同步仍可能占用较高内存；日志加载修复不代表内存问题已全部解决。

Java migration is ongoing. Live CW continuity and stop, IC-705 voice, some radio paths, real LoTW signing/upload recovery and the complete phone/bilingual/orientation matrix have not completed acceptance. Large automatic LoTW sync can still use substantial memory; restored log loading is not a full memory fix.

免费使用，无需授权。升级前备份配置和完整 ADIF 日志；发射前低功率核对 PTT、音频、ALC、功率及驻波，并保留实体停止手段。

Free, no activation. Back up settings and full ADIF logs before upgrading. Verify PTT, audio, ALC, power and SWR at low power before transmitting and keep a physical stop available.
