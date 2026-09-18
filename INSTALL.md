# 安装、升级与完整性校验

## 系统要求

- Android 7.0 或更高版本；
- 64 位 ARM 设备，CPU 架构为 `arm64-v8a`；
- 根据所用功能准备蓝牙、USB OTG、麦克风、本地网络或互联网权限；
- 发射功能要求用户具备合法有效的业余无线电操作资格、台站许可和呼号。

## 安装

1. 从本仓库 Releases 页面下载 `Radio-Echo-v0.1.5-android-arm64.apk` 和 `SHA256SUMS.txt`。
2. 按下面的方法校验 SHA-256，不要安装校验值不一致的文件。
3. 在 Android 系统设置中临时允许当前文件管理器或浏览器“安装未知应用”。
4. 打开 APK 并完成安装，安装后可关闭该来源的安装权限。
5. 首次启动时阅读并确认用户协议、隐私政策和发射安全声明。
6. 先配置呼号和网格，再按需要配置电台、LoTW、QRZ 和地图服务。

## SHA-256 校验

macOS 或 Linux：

```bash
shasum -a 256 Radio-Echo-v0.1.5-android-arm64.apk
```

Windows PowerShell：

```powershell
Get-FileHash .\Radio-Echo-v0.1.5-android-arm64.apk -Algorithm SHA256
```

版本 0.1.5 的预期 APK SHA-256：

```text
0e631cfdd7796ddafaebb65950ef0cf7b0e998c0b76510de0247c4e4dbe11610
```

官方 Android 签名证书 SHA-256：

```text
c2fad4dc5c79163f23fb80d97427c70f4a187be714546d890bf6ceea2bb819af
```

## 升级

1. 在日志页导出完整 ADIF，在设置页导出配置。
2. 不要卸载旧版，直接安装同包名、同签名的新 APK 进行覆盖升级。
3. 升级后检查呼号、设备连接、日志数量、LoTW 同步游标和证书状态。
4. 协议版本发生变化时，应用会要求重新确认。

从早期 `cn.hyperft8.mobile` 迁移时，必须先在旧应用中导出数据，再在 Radio Echo 中导入。两个包名的数据不会由 Android 自动迁移。

## 卸载与数据

卸载或清除应用数据会删除应用私有目录中的设置、日志、上传队列和已导入证书。已经提交给 LoTW 或其他第三方的数据不会随本机卸载而删除。

## 首次发射检查

安装成功不代表可以直接发射。请先使用假负载或低功率可控环境，逐项验证频率、模式、USB-D/Data 模式、PTT 释放、音频电平、ALC、功率、驻波和紧急停止。不要在无人监督状态下进行首次测试。
