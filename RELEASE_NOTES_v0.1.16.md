# Radio Echo v0.1.16

日期 / Date: 2026-11-03

## 核心更新

- **接收稳定性：** 修复界面动画历史对象持续累积的引用链，普通版连续 MIC 接收 12 分钟未复现此前的快速内存增长。
- **FT8 解码列表：** 更紧凑的单行显示，按面板宽度保留必要信息，长按查看完整详情。
- **CW Spot：** 已有呼号原位更新，滑动和按压时保持选台稳定；支持展开、搜索和手动查看新台。
- **CW 状态保护：** 区分串口写入、估算进度与电台确认；停止未确认时阻止追加拍发，未确认完成时不继续自动 CQ。

## Highlights

- **Receive stability:** removed a retained history of animated UI objects. A 12-minute MIC run with the ordinary release build did not reproduce the previous rapid memory increase.
- **FT8 decode list:** compact single-line rows adapt to pane width; long-press for full details.
- **CW Spots:** stable in-place updates and interaction holds, with expanded browsing, search and explicit new-station refresh.
- **CW status safeguards:** distinguish transport writes and estimates from radio confirmation; block further keying after an unconfirmed stop and halt automatic CQ when completion is unconfirmed.

## Installation And Validation

Android 7.0+ / API 24; `arm64-v8a`; package `cn.bi1rre.radioradioecho`;
version `0.1.16 (17)`. Free, no activation; lightweight MIT-licensed `ft8_lib`.
The ordinary APK contains no internal memory sampler or heap-snapshot tool.
761 automated tests, TypeScript, native codec/resampler/scheduled-playback and
120-cycle receive-soak checks passed, together with signed Release/R8/Lint Vital,
package/version/ABI, JNI and TrustedQSL verification.
Back up configuration and full ADIF, then install over the existing app without
uninstalling or clearing data. Verify the attached checksums and manifest.

## 已知限制 / Known Limitations

12 分钟接收测试仍有小幅内存增加，30–60 分钟、低内存手机及真实连续通联验收待完成，不代表所有 OOM 风险已解决。CW 物理停止和固件缓冲区清空仍需受控真机验证；保持操作者监督和实体停止手段。官方 FX-4CR R1.8.5（2026-05-24）不支持当前 CAT 文本 CW 快捷语，App 无法补齐该固件能力。

Small memory growth remains in the short receive test. Longer soaks, low-memory
phones, dense signals and on-air acceptance remain pending. Physical CW stop
and keyer-buffer clearing are not certified; maintain operator supervision and
a physical stop. Official FX-4CR R1.8.5 (2026-05-24) lacks the CAT text CW support
required by these presets. Native phone accessibility and some layout scenarios
also remain under validation. This is a **Pre-release**, not a fully qualified
hardware compatibility release. Earlier release assets remain unchanged.
