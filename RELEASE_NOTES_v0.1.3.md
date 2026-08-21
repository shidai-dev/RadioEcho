# Radio Echo v0.1.3

这是基于 `v0.1.2` 的 Android 设备兼容性、稳定性与版本维护更新，继续作为免费公开预览版发布，仅提供 `arm64-v8a` APK。

## 核心更新

- **USB 设备架构：** Android USB Host、串口传输、设备会话和型号协议目录完成分层，设备差异不进入 FT8、CW 或日志模块。
- **多协议 USB CAT：** 增加 Icom CI-V、Yaesu 五字节 CAT/FT-847/NewCAT、Kenwood/Elecraft、Xiegu、QRP Labs、国合和 Wolf SDR 等协议路径。没有真机证据的型号均保持“待验证”或“不可用”能力标识。
- **FX-4CR USB：** USB OTG 连接、频率控制和 CW 发射已有有限真机证据；该结果不会扩展到共用 Kenwood 协议的其他机型。
- **USB 生命周期：** 改进 USB 权限、稳定硬件身份、串口探测、物理拔出处理和资源释放，并提供不包含账号或证书秘密的诊断信息。
- **CW 与传播：** 修复 CW 操作按钮事件进入界面文本导致的闪退；RBN 改用当前 JSON 服务并支持 24 小时至 1 年的历史范围。
- **版本更新：** 设置中可控制每日 GitHub Release 检查，也可手动检查。应用不会静默安装，也不会申请未知来源安装权限。
- **界面整理：** 电台型号列表仅显示厂商、型号和选中状态，降低设备设置的信息密度。

## 已知限制

- 除 FX-4CR 的基础 USB 控制外，新增 USB 型号尚未完成逐机真机 CAT、PTT 或 CW 验收。
- USB CAT 只负责电台控制；通用 Android USB 音频接收和发射尚未完成，因此不能据此宣称完整 FT8 USB 支持。
- FT-DX10 Enhanced CAT 端口、FX-4CR 热插拔/重连/长时间稳定性和新固件 PWR/SWR 仍需真机复测。
- FT8 普通模式的弱信号、时钟偏差和蓝牙音频抖动容差仍处于现场验证阶段。
- 当前仅提供 Android `arm64-v8a`，不提供 iOS、32 位或 x86 版本。

## 安装包

```text
文件：Radio-Echo-v0.1.3-android-arm64.apk
包名：cn.bi1rre.radioradioecho
版本：0.1.3 (4)
最低 Android：API 24
目标 Android：API 35
SHA-256：d30a075d5249cb8b38dfe8fddfbfe6ea66de2fe9393daa8cab88719e512e212c
签名证书 SHA-256：c2fad4dc5c79163f23fb80d97427c70f4a187be714546d890bf6ceea2bb819af
```

## 升级提示

从旧版升级前建议导出配置和完整 ADIF。不要卸载旧版，使用同包名、同签名 APK 直接覆盖安装；升级后检查呼号、设备配置、日志数量、LoTW 同步游标和证书状态。

本版本仍为 **Pre-release**。自动发射必须由具备相应资格的操作员持续监督，并保留从电台实体控件立即停止发射的方式。
