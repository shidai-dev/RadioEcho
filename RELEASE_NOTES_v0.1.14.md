# Radio Echo v0.1.14

日期 / Date: 2026-10-22

## 核心更新

- **通联工作台：** 横屏 FT8 频谱/解码左右排列，控制区位于频谱下方，CW、FT8、日志和传播共用固定导航。工具、UTC、音源与解码状态收敛；大字体按空间换行，不强制缩小系统字体。
- **历史与草稿：** FT8 只有实际离开顶部才进入历史阅读，回到顶部恢复跟随。CW 呼号、双方报告和备注可跨切页、旋转与重启恢复；保存完成不会清掉期间新编辑的草稿。
- **操作闭环：** 查询保留已有结果并提供错误/重试；LoTW 待上传队列默认不选中，支持审核所选、二次确认及移出队列，不删除本地日志。原显式 FT8 自动上传开关保持不变。
- **FT8 契约加固：** 新会话与旧交换补确认分开，自动完成要求报告和确认的实际证据。完整音频在 PTT 前预装载，过期时隙统一拒绝；退后台撤销自动发射意图，返回不会自动重新启动发射。这些实现已通过自动化，真实连续射频交换仍待监督复测。
- **主页图片：** 中英文 README 使用各自语言的当前版本真机截图，不使用旧版界面或模拟连接状态。

## Highlights

- A less crowded FT8 landscape layout and one persistent navigation bar across all workspaces; compact decode rows and responsive large-text handling.
- History reading without unwanted jumps, return-to-latest, and CW contact drafts that survive navigation, rotation and restart.
- Consistent query recovery and explicit, selective LoTW queue review. The existing opt-in FT8 auto-upload setting is unchanged.
- Separate new calls from repeated acknowledgements; require report/confirmation evidence before completion. Preload transmit audio before PTT, reject expired slots consistently and revoke transmit intentions in the background. Continuous on-air regression remains pending.
- Updated English and Chinese README artwork captured from this Android version.

## Installation

Android 7.0+ / API 24; target API 35; `arm64-v8a` only.
Package: `cn.bi1rre.radioradioecho`; version: `0.1.14 (15)`.
Free preview, no activation; lightweight MIT-licensed `ft8_lib` backend.
Back up configuration and complete ADIF, then install the same-signature APK over the existing app without uninstalling or clearing data. Verify `SHA256SUMS.txt` and `RELEASE_MANIFEST.json`. Earlier release assets remain unchanged.

## Verification

- 706/706 automated tests and TypeScript passed.
- Native codec loopback, scheduled playback and resampling checks passed.
- Commercial Release/R8/Lint Vital, BI1RRE v2/v3 signing, package/version/ABI, 13 required JNI symbols and TrustedQSL checks passed.
- The same APK was installed on a Lenovo TB324ZC without clearing data. Native checks covered Chinese landscape navigation, history following, CW draft recovery and MIC reception. English/Chinese layout and stop-control component checks are distinct from hardware acceptance.

## Known Limitations

**Extended receive sessions may use excessive memory on some devices. This remains under investigation, not a fixed issue.** 长时间接收的高内存占用尚未修复；不建议低内存设备长时间无人值守运行。

No real radio transmission or LoTW upload was performed during release packaging. Dense-signal accuracy, continuous QSOs, final acknowledgement recovery, physical Stop/background behavior and device-specific audio routing require supervised RF retesting. Automated checks and MIC reception do not establish field compatibility or performance parity with WSJT-X/JTDX.

This is a **Pre-release**, not a stable-release certification. Keep a licensed operator and a physical stop available during testing. See the README support matrix for the limited evidence available for each radio.
