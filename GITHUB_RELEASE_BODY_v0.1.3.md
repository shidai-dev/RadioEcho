# Radio Echo v0.1.3 Android 公开预览版

本次更新重点补齐 Android USB 多电台控制架构、修复传播查询和 CW 稳定性问题，并增加应用内 GitHub 新版本检查。

## 核心变化

- 建立与 FT8、CW、日志解耦的 Android USB 串口和电台协议目录；
- 增加 Icom CI-V、Yaesu CAT、Kenwood/Elecraft、Xiegu 等实验性 USB 控制路径；
- FX-4CR USB 连接、频率控制和 CW 发射已完成有限真机验证；
- 修复 CW 操作按钮可能导致的前台闪退；
- RBN 查询迁移到当前 JSON 服务，支持更长历史范围和地图定位；
- 增加每日 GitHub Release 检查和手动检查入口，不静默下载或安装；
- 精简电台型号列表，只显示厂商、型号和选中状态。

## 下载文件

- `Radio-Echo-v0.1.3-android-arm64.apk`
- `SHA256SUMS.txt`
- `THIRD_PARTY_NOTICES.md`

APK SHA-256：

```text
d30a075d5249cb8b38dfe8fddfbfe6ea66de2fe9393daa8cab88719e512e212c
```

当前仅支持 Android `arm64-v8a`。除 FX-4CR 已记录的基础 USB 控制证据外，新增 USB 型号均为实验性支持；USB CAT 不等同于 USB 音频或完整 FT8 能力。FT8 自动流程与所有发射操作仍需持证操作员持续监督。

建议将本 Release 标记为 **Pre-release**。
