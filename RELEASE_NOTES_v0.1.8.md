# Radio Echo v0.1.8

Radio Echo v0.1.8 是免费 Android `arm64-v8a` 公开预览维护版本，重点提高 FT8 标准交换的一致性，并整理 CW 与 RBN 的户外操作界面。

## 核心更新

- **FT8 协议状态：** RX 解码与实际 TX 明文进入同一 UTC 事件账本；只有完成信号报告交换并满足合法结束条件后才保存日志，孤立 `RR73/73` 不再直接完成 QSO。
- **FT8 解码证据：** 原生层完整上送 DT、解码耗时和相对 15 秒边界的延迟，标准模式在一次 QSO 内保持固定发射音调。
- **CW 工作区：** 横屏把 CW Spot 与 QRZ 查询并列显示；竖屏默认打开 QRZ，仍可通过页签切换 Spot。
- **RBN 查询：** 默认范围改为最近 1 小时，支持 `1小时 / 6小时 / 12小时 / 24小时 / 1个月`。

## 兼容性说明

- FX-4CR、IC-705、FT-DX10、KX3 与既有设备继续沿用原验证范围；本版本没有修改 CAT、电台驱动或 CW 拍发协议。
- FT8 弱信号能力、密集多信号环境及连续自动通联仍不能等同于桌面 WSJT-X/JTDX，应继续在受控环境中验证。
- 本次公开 APK 使用 MIT 许可的 `ft8_lib` 后端，不包含深度解码测试后端。

## 安装包

```text
文件：Radio-Echo-v0.1.8-android-arm64.apk
包名：cn.bi1rre.radioradioecho
版本：0.1.8 (9)
最低 Android：API 24
目标 Android：API 35
SHA-256：c07307b594f288c12fee1f4edf579647f2a16adfa2bfe5d097d36de2dd9b153b
签名证书 SHA-256：c2fad4dc5c79163f23fb80d97427c70f4a187be714546d890bf6ceea2bb819af
```

升级前建议导出配置和完整 ADIF。不要卸载旧版，使用同包名、同签名 APK 直接覆盖安装。本版本仍为 **Pre-release**，发射操作必须由持证操作员持续监督。
