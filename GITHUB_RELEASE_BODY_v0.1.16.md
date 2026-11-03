# Radio Echo v0.1.16

## 核心更新 / Highlights

- 改善持续接收的内存增长；FT8 解码列表改为紧凑单行，长按查看详情。
- CW Spot 稳定排序、展开搜索，减少刷新时点错呼号。
- CW 拍发和停止状态更严谨，未确认停止时阻止追加拍发。

- Reduced receive-session memory growth; compact FT8 decode rows with full details on long-press.
- Stable, searchable CW Spots without automatic row jumping.
- More accurate CW completion evidence and safeguards after an unconfirmed stop.

**限制 / Limits:** 普通版 MIC 连续接收已验证 12 分钟；长时、低内存手机和 CW 物理停止仍待验收，不宣称所有内存或固件问题已解决。Official FX-4CR R1.8.5 does not support these CAT text CW presets. Longer soak and supervised radio acceptance remain pending.

免费、无需授权；Android 7.0+、arm64，轻量 `ft8_lib`。版本 **0.1.16 (17)**，继续作为 **Pre-release** 发布。升级前备份配置和完整 ADIF，覆盖安装，不卸载、不清除数据。

Download the independent APK below, not GitHub's source archive. Back up settings
and ADIF before a retaining-data upgrade. Keep operator supervision and a physical
stop available. See the attached bilingual release notes for details.
