# 掌上部费

掌上部费是一款本地优先的 Android 部费与收支记录应用。本仓库用于分发正式安装包和记录发布校验信息，不包含应用源码、签名私钥或用户账本数据。

## 当前版本

- 版本：`1.0.3`
- versionCode：`166`
- Android 包名：`com.pocketledger.app`
- 已完成验证的平台：Android 16 / API 36
- APK 签名：APK Signature Scheme v3，RSA 4096 位

> 工程的 `minSdk` 为 API 31，但 Android 12–15 尚未完成正式兼容性验收，因此本版本只对 Android 16 的已验证范围作出声明。

## 下载与安装

下载 [掌上部费-1.0.3.apk](Releases/%E6%8E%8C%E4%B8%8A%E9%83%A8%E8%B4%B9-1.0.3.apk)，然后在 Android 系统中允许当前文件来源安装未知应用。

安装或升级前建议先在应用内完成数据备份。由正式版 `1.0.2` 原位升级到 `1.0.3` 的同签名安装已经在 Android 16 上验证；其他来源或不同签名的旧安装包可能无法直接覆盖安装。

## 完整性校验

APK 文件：`Releases/掌上部费-1.0.3.apk`

SHA-256：

```text
AFA8F013CBF090E4FBA5BB7D6EF6067CBB089728410D009E0A6DA30C2CF074C9
```

也可以使用仓库中的 [SHA256SUMS.txt](Releases/SHA256SUMS.txt) 进行校验。在 Windows PowerShell 中运行：

```powershell
Get-FileHash -Algorithm SHA256 .\掌上部费-1.0.3.apk
```

## 验证状态

- `verified`：正式 APK 已签名、压缩并通过签名校验；Android 16 上已验证同签名升级、安装后 APK 字节一致、正式包不可调试、冷启动无 fatal/ANR。
- `partial`：完整三语言无障碍矩阵、低存储/故障注入/长时间稳定性和自然 MIUI 后台时序仍未全部关闭。
- `blocked`：第二台设备的跨设备 ZIP 迁移验证仍冻结。

## 隐私说明

应用采用本地优先设计。用户仍应自行妥善保管应用内导出的备份文件，不要将真实账本备份公开上传到 GitHub。
