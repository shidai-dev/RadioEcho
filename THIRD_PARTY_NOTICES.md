# Radio Echo 第三方许可与非关联声明

本文件适用于 `Radio-Echo-v0.1.0-android-arm64.apk`。Radio Echo 自有代码为 BI1RRE 版权所有；本文件只说明第三方组件权利，不向 Radio Echo 自有代码授予开源许可。

## 发行边界

当前 APK 使用 MIT 许可的 `ft8_lib` 作为 FT8 编解码组件。

## 主要第三方组件

- `ft8_lib`, Copyright (c) 2018 Kārlis Goba, MIT License；
- TrustedQSL/libtqsl, Copyright (C) 2001-2015 American Radio Relay League, Inc. and portions Copyright (C) 2003-2026 The TrustedQSL Developers, TrustedQSL License Terms and Conditions；
- React Native、React、Expo、Expo Modules 和 `@expo/vector-icons`，适用随包 MIT 许可证；
- `react-native-svg`、`react-native-tcp-socket` 和 `@react-native-community/netinfo`，适用随包 MIT 许可证；
- `react-native-ble-plx`，适用其随包 Apache License 2.0；
- AndroidX、Kotlin、Hermes、OpenSSL 及其依赖，适用其各自许可证和免责声明；
- Big CTY `cty.dat` 数据来源为 `country-files.com`，当前内置数据库修订标记为 `VER20260714`；
- DXCC 简体/繁体参考资料来源作者 VR2UPU、BD7MJO，中国呼号区资料按随包来源说明使用。

发布附件中的 `licenses/` 目录保留了上述直接运行时组件的许可文本；APK 内 `assets/licenses/` 同时保留了 `ft8_lib` 和 TrustedQSL 的完整许可文本。其他运行时依赖的版权和许可继续以其上游发行材料为准。本项目不会使用 Radio Echo 条款覆盖第三方已经授予的权利。

## ft8_lib MIT License

Copyright (c) 2018 Kārlis Goba

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## TrustedQSL License Terms and Conditions

TrustedQSL 的完整、未删节许可条件和免责声明见 [`licenses/TrustedQSL-LICENSE.txt`](licenses/TrustedQSL-LICENSE.txt)，并保留在 APK 内。

## 商标和第三方服务

LoTW、TrustedQSL、ARRL、Icom、FX-4CR、QRZ、天地图、PSK Reporter、WSPR、Reverse Beacon Network 及其他名称、产品标识和商标归各自权利人所有。Radio Echo 的兼容或接入不表示获得其认可、赞助、认证或合作授权。

许可问题可联系 `BI1RRE@163.com`。
