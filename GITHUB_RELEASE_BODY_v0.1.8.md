# Radio Echo v0.1.8 Android 公开预览版

本次版本重点收口 FT8 标准交换状态和解码时序证据，并改善 CW/RBN 户外操作布局。

## 核心变化

- FT8 使用统一的收发事件账本判断交换阶段与完成状态，减少乱序消息和孤立 `RR73/73` 导致的错误日志；
- 补齐 FT8 解码 DT、耗时和相对 UTC 周期的延迟信息，标准 QSO 在会话内保持同一发射音调；
- CW 横屏将 Spot 与 QRZ 调整为同一双栏工作区，竖屏默认显示 QRZ；
- RBN 默认查询最近 1 小时，并提供 1 小时、6 小时、12 小时、24 小时和 1 个月范围。

## 下载文件

- `Radio-Echo-v0.1.8-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK SHA-256：

```text
c07307b594f288c12fee1f4edf579647f2a16adfa2bfe5d097d36de2dd9b153b
```

当前仅支持 Android `arm64-v8a`。本版本仍为 **Pre-release**；自动发射应先在低功率、假负载或可控环境中验证，并由具备相应资格的操作员持续监督。
