# Radio Echo

Radio Echo 是由业余无线电爱好者 `BI1RRE` 独立开发维护的 Android 业余无线电辅助应用，提供电台连接、CW、FT8、ADIF 日志、LoTW 和传播信息等功能。

> 当前仓库仅用于发布官方二进制 APK、使用文档和问题反馈，不提供 Radio Echo 自有源代码。免费使用不代表软件已按开源许可证发布。

## 下载

请从本仓库直接下载 [`Radio-Echo-v0.1.0-android-arm64.apk`](Radio-Echo-v0.1.0-android-arm64.apk)，或从 [Releases](../../releases) 页面下载同名附件。当前版本为公开预览版，发布 Release 时应勾选 GitHub 的 **Pre-release**，不建议从第三方网盘、群文件或重新打包站点安装。

发布附件：

- `Radio-Echo-v0.1.0-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK 信息：

| 项目 | 内容 |
| --- | --- |
| 应用名称 | Radio Echo |
| 版本 | 0.1.0 (versionCode 1) |
| Android 包名 | `cn.bi1rre.radioradioecho` |
| 最低系统 | Android 7.0 / API 24 |
| 目标系统 | Android API 35 |
| CPU 架构 | `arm64-v8a` |
| 授权状态 | 免费测试版，无试用倒计时，无授权码 |
| FT8 后端 | MIT 许可的 `ft8_lib` 轻量后端 |

## 当前支持范围

- FX-4CR：Bluetooth SPP CAT、CW 键控及兼容音频链路。
- Icom IC-705：Icom WLAN Remote，以及 USB CI-V 控制路径。
- CW：快捷键控、频率控制、WPM、手动通联日志和 DX Cluster Spot。
- FT8：接收频谱、15 秒周期、轻量解码、手动或自动通联流程。
- 日志：本地 ADIF、导入导出、编辑删除、LoTW 历史同步和手动确认上传。
- 传播：PSK Reporter、WSPR 和 Reverse Beacon 数据展示。

其他电台、固件、Android 厂商系统和音频路由尚未完成全面验证。兼容列表表示已有实现路径，不代表所有组合都已通过实地验收。

## 安装与升级

完整步骤见 [INSTALL.md](INSTALL.md)。升级前请在应用内导出配置和 ADIF 日志。早期包名 `cn.hyperft8.mobile` 与当前包名不同，Android 不会自动迁移旧应用私有数据。

## 发射安全

本应用不授予业余无线电操作资格、台站执照、呼号或监管许可。首次发射前必须在低功率、可控环境核对频率、模式、PTT、音频、ALC、功率和驻波，并确保能够从电台实体控件立即停止发射。

使用自动 CQ、自动应答或连续发射时，实际操作人必须持续监督。发生错误频率、异常带宽、PTT 无法释放、设备断连、有害干扰或状态不确定时，应立即停止发射。

详见 [业余无线电合规与发射安全声明](legal/RADIO_COMPLIANCE_NOTICE.zh-CN.md)。

## 隐私与联网服务

Radio Echo 不设应用账户和自有云端日志库。本地日志、证书、音频和设备配置默认在设备本机处理。只有在用户主动配置或使用 LoTW、QRZ、天地图、Telnet、PSK Reporter、WSPR、RBN 或电台网络连接时，应用才会直接连接相应第三方。

请勿在公开 Issue 中上传 LoTW/QRZ/Icom 密码、P12 文件或密码、天地图 API Key、完整配置备份以及包含个人信息的原始日志。

详见 [用户服务协议](legal/USER_SERVICE_AGREEMENT.zh-CN.md) 和 [隐私政策](legal/PRIVACY_POLICY.zh-CN.md)。

## 软件许可

本仓库发布的是 Radio Echo 免费二进制测试版，不提供 Radio Echo 自有源代码。用户可从官方 Release 下载并在自己的 Android 设备上安装使用。第三方组件继续适用各自许可证。

详见 [二进制发行许可](LICENSE)、[二进制发行声明](BINARY_DISTRIBUTION_NOTICE.md) 和 [第三方许可声明](THIRD_PARTY_NOTICES.md)。

## 反馈与支持

- 普通缺陷：使用仓库的 Bug report 模板提交 Issue。
- 安全问题或敏感材料：发送邮件至 `BI1RRE@163.com`，不要公开提交。
- 提交前请阅读 [SUPPORT.md](SUPPORT.md) 和 [SECURITY.md](SECURITY.md)。

本项目由个人爱好者利用业余时间维护，不承诺服务等级、修复期限或对所有设备提供兼容支持。

## English summary

Radio Echo is a binary-only Android amateur-radio companion maintained by BI1RRE. This repository distributes official APK files and documentation but does not publish proprietary source code. The current preview is free to use, requires no activation code, targets arm64 Android devices, and must be operated under the user's local amateur-radio laws and station authorization.
