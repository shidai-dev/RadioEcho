# Radio Echo v0.1.14 Android 公开预览版

## 核心更新

- **通联工作台：** FT8 横屏频谱与解码左右分区，控制区置于频谱下方，四页统一固定导航；精简状态和解码行，改善中英文与大字体布局。
- **阅读与操作恢复：** FT8 翻历史不再被新消息打断，回到顶部恢复跟随；CW 未保存草稿支持切页、旋转与重启恢复；查询支持明确重试，LoTW 队列可逐条审核。
- **FT8 流程加固：** 区分新呼叫与重复确认，收紧报告/完成证据；调整发射音频预装载、过期时隙准入与后台停止行为。主页配图全部换成当前版本中英文真机截图。

## Highlights

- A cleaner FT8 workspace with side-by-side spectrum/decodes in landscape and consistent navigation across all four tabs.
- Stable history reading, return-to-latest, persistent CW drafts, clearer query recovery and selective LoTW queue review.
- Hardened FT8 exchange evidence, repeated acknowledgements, preloaded transmit audio, expired-slot admission and background stop handling. Updated English/Chinese screenshots from this Android build.

## 验证与限制 / Validation And Limitations

706 automated tests, TypeScript, native codec/playback/resampling checks and signed APK verification passed. Tablet installation, navigation and MIC reception were checked. These checks **do not certify on-air operation**; continuous RF exchanges and hardware-specific audio routing still require supervised retesting.

**已知问题：长时间接收在部分设备上可能出现较高内存占用，正在调查，尚未修复。**
**Known issue: extended receive sessions may consume excessive memory on some devices; investigation remains open.**

仍为 **Pre-release**，免费且无需授权码；Android 7.0+，仅 `arm64-v8a`，轻量 `ft8_lib` 后端。升级前备份配置及完整 ADIF，覆盖安装同签名 APK。保持持证操作员监督和物理停止手段，不建议低内存设备长时间无人值守运行。

Download the independent APK asset, not GitHub's source archive. Back up configuration and complete ADIF before upgrading. Keep an operator present and a physical means to stop transmission. Previous release assets are unchanged.
