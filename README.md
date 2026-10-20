# Instant 下载与更新

Instant 是一款原生 macOS 键盘启动器，提供应用与文件搜索、剪贴板历史、Snippet、Workflow 和 Finder 文件操作。

此仓库只发布安装包、校验文件和更新说明。源码仓库保持私有。

## 下载

[查看最新正式版本](https://github.com/dengqiangxi/instant-releases/releases/latest)

下载 `Instant-macos-universal.zip`，解压后将 `Instant.app` 放入固定位置（例如 `/Applications`），再打开应用。

- 支持 macOS 13 及以上。
- 主程序和 Finder 扩展均包含 Intel（x86_64）与 Apple Silicon（arm64）。
- 更新时先退出旧版，再替换同一路径的应用；用户配置与历史数据独立保存。

## 校验下载

同时下载 `Instant-macos-universal.zip.sha256`，在下载目录执行：

```sh
shasum -a 256 -c Instant-macos-universal.zip.sha256
```

## 签名与权限

当前版本使用 ad hoc 签名，未经过 Apple 公证。macOS 可能要求手动允许打开；更新后辅助功能和 Finder 扩展可能需要重新授权。

本仓库不包含源码；公开安装包不代表授予开源许可。
