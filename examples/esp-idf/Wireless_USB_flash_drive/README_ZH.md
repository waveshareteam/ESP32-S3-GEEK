# USB 无线磁盘

[English](README.md) | **简体中文**

## 功能

通过 USB 大容量存储和 Wi-Fi 网页访问同一存储介质。

## 硬件需求

ESP32-S3-GEEK 开发板及带 USB 接口的主机。选择外置存储时需要 microSD 卡。

## 怎么运行

在 ESP-IDF 环境中运行 `idf.py set-target esp32s3`。如需使用 microSD，请在 `idf.py menuconfig` 中选用外置 SD 卡，再运行 `idf.py build flash`。

## 预期现象

主机识别可移动磁盘。连接开发板热点后，可在网页中查看和传输文件。

## 常见问题

USB 与网页间的文件列表可能不同步。请先安全弹出，再重新挂载以刷新列表。使用隔离网络测试，默认热点没有密码。