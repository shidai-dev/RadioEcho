# Security Policy

## Supported versions

Only the latest GitHub pre-release APK is supported for security fixes. Older preview builds may contain known defects and should be upgraded after backing up configuration and ADIF logs.

## Reporting a vulnerability

Send security reports privately to `BI1RRE@163.com` with the subject `Radio Echo Security Report`.

Please include:

- Radio Echo version and APK SHA-256;
- Android version and device model;
- affected feature and reproducible steps;
- expected and observed behavior;
- sanitized logs or screenshots;
- whether radio transmission, PTT, credentials, certificates or local files are affected.

Do not open a public Issue containing:

- LoTW, QRZ, Icom or Telnet passwords;
- P12/TQ5/TQ8 files or certificate passwords;
- Tianditu API keys;
- complete configuration backups;
- private signing keys or personal QSO data;
- a working exploit before a fix is available.

This is a personal project without a guaranteed response SLA. Reports will be acknowledged and prioritized according to user safety, unintended transmission risk, credential exposure and data loss impact.

## APK authenticity

Official release APKs use package name `cn.bi1rre.radioradioecho` and the signing certificate SHA-256 below:

```text
c2fad4dc5c79163f23fb80d97427c70f4a187be714546d890bf6ceea2bb819af
```

Do not install an APK with a different package signature or a SHA-256 that does not match the release checksum.
