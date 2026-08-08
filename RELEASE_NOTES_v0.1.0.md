# Radio Echo v0.1.0

首个公开 Android 预览版本。此版本免费使用、无需授权码，仅提供 `arm64-v8a` 二进制 APK，不提供 Radio Echo 自有源代码。

## 主要功能

- FX-4CR Bluetooth SPP 和 Icom IC-705 WLAN/USB 连接路径；
- CW 快捷键控、WPM、频率控制、Spot 和手动日志；
- FT8 频谱、周期显示、轻量解码及通联状态流程；
- 本地 ADIF 日志、搜索、编辑、导入导出和地图展示；
- LoTW 历史同步、双方确认状态和用户手动确认上传；
- QRZ、天地图、PSK Reporter、WSPR 和 Reverse Beacon 可选接入；
- 中英文界面、配置备份和本地优先的数据处理。

## 重要变化

- 当前公开包不启用授权码和三天试用，安装后可直接使用完整功能；
- LoTW 页面收敛为“同步”和“审核上传”两个日常操作，低频兼容项默认折叠；
- 包名为 `cn.bi1rre.radioradioecho`，与早期 `cn.hyperft8.mobile` 不共享应用数据；
- 当前 FT8 使用 MIT 许可的 `ft8_lib` 编解码组件。

## 已知限制

- 当前仅提供 `arm64-v8a` APK，暂不提供 iOS、x86 或 32 位 Android 版本；
- FT8 弱信号能力、连续自动通联和复杂多信号环境仍需更多实地验证，不能代替 WSJT-X/JTDX 等桌面软件；
- IC-705 与 FX-4CR 以外的设备未完成正式兼容验收；
- 不同 Android 厂商的蓝牙音频、USB 权限和后台限制可能影响接收稳定性；
- LoTW 上传一旦被服务端接受通常无法由应用撤回，必须在上传前核对日志；
- 网络服务可能受账号权限、配额、地区网络和第三方接口变化影响。

## 安装包

```text
文件：Radio-Echo-v0.1.0-android-arm64.apk
包名：cn.bi1rre.radioradioecho
版本：0.1.0 (1)
最低 Android：API 24
目标 Android：API 35
SHA-256：8f0a757ffc7a51f308bb6c663dc679e752c218fe47ca5bf4a86b78d2ff8ecf9f
签名证书 SHA-256：c2fad4dc5c79163f23fb80d97427c70f4a187be714546d890bf6ceea2bb819af
```

## 升级提示

升级前导出配置和完整 ADIF。请从官方 GitHub Release 下载并核对 SHA-256。第一次使用发射功能时应在低功率、可控环境完成完整安全验证。

问题反馈请使用仓库 Issue 模板；涉及密码、证书、API Key 或安全漏洞时请发送邮件至 `BI1RRE@163.com`。
