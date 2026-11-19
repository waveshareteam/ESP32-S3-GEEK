# ESP32-S3-GEEK Firmware

[简体中文](README_ZH.md)

| Firmware | Version date | Flash offset | Purpose |
| --- | --- | --- | --- |
| [ESP32-S3-GEEK_FactoryOnly_20260409.bin](ESP32-S3-GEEK_FactoryOnly_20260409.bin) | 2026-04-09 | `0x0` | Factory test firmware for ESP32-S3-GEEK with 16 MB Flash |

Hold BOOT while connecting the board over USB, then release it. Replace `PORT` with the board’s serial port and run the following command from this directory. Reconnect the board after flashing.

```sh
python -m esptool --chip esp32s3 --port PORT write-flash 0x0 ESP32-S3-GEEK_FactoryOnly_20260409.bin
```
