# Radio Echo v0.1.13 Android 公开预览版

## 核心更新

- 修正 USB 发射音频误走扬声器的已确认路由链路，增加每轮端点重绑定和断路保护。
- 工作频率跟随电台回读，补齐 DX10 发射功率/驻波表计；表计为标定估算，需与电台面板核对。
- FT8 横屏将导航、通联摘要和呼叫/停止合为单行底栏，给频谱与解码腾出更多空间。

## Highlights

- Corrected the confirmed USB TX routing/policy failure path, with per-cycle
  output rebinding and route-loss protection.
- Live radio dial synchronization and DX10 TX power/SWR meter estimates.
- A single landscape FT8 footer combines navigation, QSO summary and Call/Stop.

免费预览，无需授权码。Android 7.0+，仅 `arm64-v8a`，正式签名，可保留数据覆盖升级；请先备份配置和完整 ADIF。

**仍为 Pre-release，现场修复效果尚待真机复测。** 自动化/组件预览不等于 Android 原生或射频验收；表计不是校准仪表，不改变发射许可与安全要求。

Free preview with the lightweight `ft8_lib` backend. Native-device/RF retesting
remains pending; automated checks do not certify hardware routing or meter
accuracy. Use supervised, low-power controlled testing and retain a physical stop.

请下载附件中的独立 APK，而非 GitHub 的源码压缩包。
