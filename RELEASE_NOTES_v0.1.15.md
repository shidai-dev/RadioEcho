# Radio Echo v0.1.15

日期 / Date: 2026-10-24

## 核心更新

**改善手机日志页的可用空间。** 短横屏查询、新增和同步合并为紧凑工具栏，竖屏把日志/地图/DXCC 选择与搜索放在同一行；减少顶部设备栏和底部导航的留白，保留关键操作的触摸尺寸。搜索不因窗口变化重新挂载，表单高度适应更短的窗口。本版不修改电台协议、音频、FT8 状态机、日志数据或 LoTW 上传策略。

## Highlights

**More room for logs on phones.** A compact landscape toolbar and a combined
view picker/search row in portrait leave more space for records. Shared device
and navigation bars use less vertical padding, search retains its input node
across window changes, and forms fit shorter windows. Radio protocols, audio,
FT8 sequencing, log data and LoTW upload policies are unchanged.

## Installation And Verification

Android 7.0+ / API 24; target API 35; `arm64-v8a` only.
Package: `cn.bi1rre.radioradioecho`; version: `0.1.15 (16)`.
Free preview, no activation; lightweight MIT-licensed `ft8_lib` backend.
TypeScript and 709 automated tests passed, with 18 bilingual log component
checks and 16 shared navigation/stop checks. Commercial Release/R8/Lint Vital,
BI1RRE v2/v3 signature, version/ABI, JNI and TrustedQSL checks passed.

Back up full configuration and ADIF, then install the same-signature APK over
the existing app without uninstalling or clearing data. Verify `SHA256SUMS.txt`
and `RELEASE_MANIFEST.json`. Earlier release assets remain unchanged.

## Known Limitations

**手机原生系统栏、输入法、大字体和 TalkBack 仍待验收。** 组件检查不能替代 Android 真机验证，不代表全应用手机适配已完成。

**长时间接收的高内存占用仍在调查，尚未修复。** 不建议低内存设备长时间无人值守运行。

Native phone system bars, keyboards, large text and TalkBack still require
acceptance testing. Component checks do not certify all phone layouts or RF
operation. Extended-receive high memory remains unresolved. No transmission or
LoTW upload was performed during packaging. Keep operator supervision and a
physical means to stop transmission. This remains a **Pre-release**.
