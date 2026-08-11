# 【Android 预览版】Radio Echo：面向便携通联的 CW、FT8 与日志工具

![Radio Echo 便携电台工作台](https://raw.githubusercontent.com/shidai-dev/RadioEcho/main/promo/radio-echo-forum-cover.png)

各位老师好，我是 **BI1RRE**。

过去一段时间，我一直在开发一款面向业余无线电便携使用场景的 Android 应用：**Radio Echo**。

做这个项目的初衷很简单：户外架台或临时操作时，携带电脑并不总是方便。我希望通过一台 Android 手机或平板，完成电台连接、CW 操作、FT8 收发、传播查询以及通联日志管理等常用工作。

Radio Echo 目前仍是个人维护的预览版本。它并不是为了取代 WSJT-X、JTDX 等成熟桌面软件，而是希望成为一套更加轻量、适合便携台和移动设备的无线电操作工具。

## 目前包含的功能

### 电台连接与控制

- FX-4CR 蓝牙 SPP 连接
- Icom IC-705 WLAN Remote 连接
- Icom IC-705 USB 连接
- 根据设备能力控制频率、模式和 PTT，并接入接收音频
- 设备连接采用独立适配结构，便于后续增加其他电台

### CW 操作台

- 常用波段和频率快速切换
- 手动频率调节与 CW 键速设置
- 可编辑的常用拍发内容
- 自动 CQ 与轮间等待
- RBN、DX Cluster Spot 和国内外 Telnet 节点
- QRZ 呼号查询与 CW 通联日志记录

### FT8

- 实时频谱和 15 秒时隙显示
- FT8 接收、轻量解码和标准通联明文
- CQ、回应、信号报告与结束流程
- 结合本地及 LoTW 历史记录标识已通联呼号
- 新呼号、新 DXCC 等候选目标提示
- 通联完成后保存日志

FT8 仍然是当前重点验证的部分。弱信号能力、复杂多信号环境和连续自动通联，与 WSJT-X、JTDX 等桌面软件仍有差距，欢迎实际使用后提供日志协助改进。

### 日志、LoTW 与传播查询

- 本地 ADIF 日志保存、搜索、编辑和删除
- ADIF 导入、导出及手动新增日志
- LoTW 历史同步、双方确认状态与上传队列管理
- 世界通联地图和 DXCC 统计
- PSK Reporter、WSPR 与 Reverse Beacon Network 传播查询
- 中英文界面以及设置备份和恢复

![Radio Echo 功能界面](https://raw.githubusercontent.com/shidai-dev/RadioEcho/main/promo/radio-echo-ui-nine-grid.jpg)

## 当前版本

- **版本：** Radio Echo v0.1.0
- **系统：** Android 7.0 及以上
- **架构：** arm64-v8a
- **费用：** 当前预览版免费使用，无需授权码

## 下载与反馈

GitHub Release：

https://github.com/shidai-dev/RadioEcho/releases/latest

项目主页及问题反馈：

https://github.com/shidai-dev/RadioEcho

## 已知限制

- 当前只提供 Android 64 位 APK，暂不提供 iOS 和 32 位版本。
- IC-705、FX-4CR 以外的电台尚未完成正式兼容验收。
- 不同 Android 厂商的蓝牙、USB 权限和后台策略可能影响稳定性。
- QRZ、天地图和 LoTW 等服务需要用户自己的账号、证书或 API Key。
- LoTW 日志一旦被服务端接受通常无法撤回，上传前请认真核对。
- 自动发射必须由具备相应操作资格的用户在监管状态下使用。

反馈问题时，最好附上手机型号、Android 版本、电台型号、连接方式和问题发生时间。请不要公开上传密码、P12 证书、LoTW 账号或 API Key。

这是一个由个人利用业余时间维护的项目，难免还有需要继续打磨的地方。欢迎各位老师试用、拍砖并提出建议。

**73！**

**BI1RRE**  
**Radio Echo**

> 界面拼图来自 v0.1.0 后续测试构建；部分细节可能与当前公开 APK 不同，实际功能以对应 Release Notes 为准。
