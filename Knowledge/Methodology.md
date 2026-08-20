# Methodology

1. 从原工程正式发布目录选择已签名、已验证的 APK，不重新构建或覆盖原始产物。
2. 对复制前后的 APK 执行 SHA-256 比对。
3. 使用 Android Build Tools 校验签名、包名、版本和 SDK 信息。
4. 在独立 Git 仓库中提交分发文件，避免把原工程源码、构建缓存、密钥或账本数据一并上传。
5. 将 APK 同时作为仓库文件和 GitHub Release Asset 发布，并在 README 记录验证边界。
