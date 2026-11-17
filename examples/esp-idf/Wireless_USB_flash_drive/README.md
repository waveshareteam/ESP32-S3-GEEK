# USB wireless disk

**English** | [简体中文](README_ZH.md)

## What It Does

Exposes storage through USB mass storage and a Wi-Fi web interface.

## Hardware Required

An ESP32-S3-GEEK and a USB host. A microSD card is required when external storage is selected.

## How to Run

In an ESP-IDF shell, run `idf.py set-target esp32s3`. To use microSD, select external SD storage in `idf.py menuconfig`, then run `idf.py build flash`.

## Expected Result

The host mounts a removable drive. Connect to the board’s access point to browse and transfer files in a browser.

## Troubleshooting

USB and web file listings may lag behind each other. Eject and remount the USB disk to refresh it. Use an isolated network because the default access point has no password.