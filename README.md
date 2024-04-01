# Shelly convert to HAA
This guide explains how to convert Shelly ESP32 and ESP32-C3 driven devices to [HAA firmware](https://github.com/RavenSystem/esp-homekit-devices/wiki)

## :warning: **There is no way back to Shelly firmware if you have initiated the convert process!**

## Requisites
- Download corresponding ZIP file from [Releases](https://github.com/RavenSystem/mgos32toHAA/releases).
- Shelly doesn't need to be updated to latest firmware version.
- Shelly doesn't need to be connected to your WiFi network.

## Instructions
1. Connect to Shelly device and open its web interface.
2. Navigate to `Settings -> Firmware`, and drag & drop the ZIP file in the firmware update area.
3. Click the `Update` button.
4. Wait until Shelly web interface tries to reload, and wair 30 seconds more to let new firmware to do the process.
5. Now, a `HAA-XXXXXX` WiFi HotSpot should be visible to start the [HAA Installation steps](https://github.com/RavenSystem/esp-homekit-devices/wiki/installation#installing-haa).

Most common scripts are preloaded for several Shelly models, normally with switch functions.
