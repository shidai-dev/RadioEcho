# [Android Preview] Radio Echo: CW, FT8 and Logging for Portable Operation

![Radio Echo portable radio console](https://raw.githubusercontent.com/shidai-dev/RadioEcho/main/promo/radio-echo-forum-cover.png)

Hello, I am **BI1RRE**.

For some time I have been developing **Radio Echo**, an Android application designed for portable amateur-radio operation.

The idea is straightforward: carrying a computer is not always convenient during field or temporary operation. Radio Echo aims to bring radio connectivity, CW operation, FT8, propagation reports and QSO logging to an Android phone or tablet.

Radio Echo is currently a personal preview project. It is not intended to replace mature desktop applications such as WSJT-X or JTDX. Its focus is a lighter workflow for portable stations and mobile devices.

## Current Features

### Radio connectivity and control

- FX-4CR over Bluetooth SPP
- Icom IC-705 over WLAN Remote
- Icom IC-705 over USB
- Frequency, mode and PTT control where supported, plus receive-audio input
- An adapter-based device layer prepared for additional radios

### CW console

- Quick band and frequency selection
- Manual frequency adjustment and CW speed control
- Editable CW message presets
- Automatic CQ with a configurable interval between transmissions
- RBN and DX Cluster spots with selectable international and China-based Telnet nodes
- QRZ callsign lookup and CW QSO logging

### FT8

- Live spectrum and 15-second slot display
- FT8 receive, lightweight decoding and standard exchange messages
- CQ, reply, signal-report and closing sequences
- Worked-call matching against local and LoTW history
- New-callsign and new-DXCC candidate hints
- Local logging after a completed QSO

FT8 remains an active field-test area. Weak-signal performance, dense multi-signal conditions and unattended sequencing are not yet equivalent to mature desktop software such as WSJT-X or JTDX. Field logs and reproducible reports are welcome.

### Logging, LoTW and propagation

- Local ADIF storage, search, editing and deletion
- ADIF import/export and manual QSO entry
- LoTW history synchronization, confirmation status and upload-queue review
- World QSO map and DXCC statistics
- PSK Reporter, WSPR and Reverse Beacon Network queries
- Chinese and English UI, plus settings backup and restore

![Radio Echo interface overview](https://raw.githubusercontent.com/shidai-dev/RadioEcho/main/promo/radio-echo-ui-nine-grid.jpg)

## Current Release

- **Version:** Radio Echo v0.1.0
- **Requirement:** Android 7.0 or later
- **Architecture:** arm64-v8a
- **Price:** The current preview is free and requires no license code

## Download and Feedback

GitHub Releases:

https://github.com/shidai-dev/RadioEcho/releases/latest

Project page and issue tracker:

https://github.com/shidai-dev/RadioEcho

## Known Limitations

- The current build is Android arm64 only. iOS and 32-bit Android builds are not available.
- Radios other than the IC-705 and FX-4CR have not completed compatibility acceptance testing.
- Bluetooth behavior, USB permissions and background restrictions vary between Android vendors.
- QRZ, Tianditu and LoTW require the user's own account, certificate or API key.
- QSOs accepted by LoTW normally cannot be withdrawn, so logs must be reviewed before upload.
- Automatic transmission must only be used under the supervision of a properly licensed operator.

When reporting an issue, please include the Android device and version, radio model, connection type and approximate occurrence time. Never post passwords, P12 certificates, LoTW credentials or API keys publicly.

This is a personal project maintained in spare time, so there is still plenty to refine. Testing reports and constructive feedback are very welcome.

**73!**

**BI1RRE**  
**Radio Echo**

> The interface collage was captured from a post-v0.1.0 test build. Some details may differ from the currently published APK; the release notes for each APK are authoritative.
