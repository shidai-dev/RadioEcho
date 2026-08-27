# Radio Echo v0.1.4

这是基于 `v0.1.3` 的设备控制与 FT8 发射稳定性更新，继续作为免费公开预览版发布，仅提供 `arm64-v8a` APK。

## 核心更新

- **FT-DX10 USB CW：** Enhanced 串口继续负责 CAT，Standard 串口通过 DTR 执行点划时序。电台设置 `PC KEYING=DTR` 后，快捷语已完成真机拍发验证。
- **FX-4CR 蓝牙：** 连接时根据真实回包识别链路能力。新版蓝牙模块无回包时保留写控制并停止状态及 PWR/SWR 轮询；后续固件恢复回包后会自动启用完整状态能力。
- **FT8 自动流程：** 自动 CQ 使用统一标准明文，定向 CQ、六位网格及发射资源短暂占用不再轻易丢失下一周期决策。
- **发射时序分层：** PTT 提前量与稳定时间由设备传输策略提供，FT8 和 CW 业务层不包含具体电台型号判断。

## 已知限制

- FX-4CR USB 完整回读、PWR/SWR 实值和长时间稳定性仍需真机验收。
- IC-705 USB FT8 连续自动发射和 FT-DX10 USB FT8 射频频谱形态仍需受控复测。
- 通用 Android USB 音频接入尚未完成；USB CAT 能连接不代表该组合已经具备完整 FT8 收发能力。
- 其他没有真机证据的 USB 电台目录继续标记为实验性支持。
- 当前仅提供 Android `arm64-v8a`，不提供 iOS、32 位或 x86 版本。

## 安装包

```text
文件：Radio-Echo-v0.1.4-android-arm64.apk
包名：cn.bi1rre.radioradioecho
版本：0.1.4 (5)
最低 Android：API 24
目标 Android：API 35
SHA-256：e4a322f95eb316a1bff8f2ffe283fda1f71670cc0a0560557946a823ae24d7ff
签名证书 SHA-256：c2fad4dc5c79163f23fb80d97427c70f4a187be714546d890bf6ceea2bb819af
```

## 升级提示

升级前建议导出配置和完整 ADIF。不要卸载旧版，使用同包名、同签名 APK 直接覆盖安装；升级后检查呼号、设备配置、日志数量、LoTW 同步游标和证书状态。

本版本仍为 **Pre-release**。自动发射必须由具备相应资格的操作员持续监督，并保留从电台实体控件立即停止发射的方式。
