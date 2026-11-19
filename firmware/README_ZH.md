# ESP32-S3-GEEK 固件

[English](README.md)

| 固件 | 版本日期 | 烧录偏移 | 用途 |
| --- | --- | --- | --- |
| [ESP32-S3-GEEK_FactoryOnly_20260409.bin](ESP32-S3-GEEK_FactoryOnly_20260409.bin) | 2026-04-09 | `0x0` | 适用于配备 16 MB Flash 的 ESP32-S3-GEEK 的出厂测试固件 |

按住 BOOT 键，通过 USB 连接开发板，再松开按键。将 `PORT` 替换为开发板的串口，在本目录运行下列命令。烧录完成后重新连接开发板。

```sh
python -m esptool --chip esp32s3 --port PORT write-flash 0x0 ESP32-S3-GEEK_FactoryOnly_20260409.bin
```
