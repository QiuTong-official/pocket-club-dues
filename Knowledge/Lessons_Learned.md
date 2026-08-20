# Lessons Learned

- GitHub 将纯中文仓库标识规范化为空标识并最终显示为 `-`，因此仓库 URL 使用稳定的 ASCII 名称 `pocket-club-dues`，中文产品名保留在 README、仓库说明和 Release 标题中。
- APK 为 57.34 MiB，虽然低于 GitHub 100 MB 单文件硬限制，但超过 50 MB 建议值；GitHub Release 更适合作为主要下载入口。
- 发布仓库应与源码工程隔离，避免脏工作树、构建缓存、签名材料和真实数据被误提交。
