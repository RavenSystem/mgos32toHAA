# Shelly convert to HAA
This guide explains how to convert Shelly ESP32 and ESP32-C3 driven devices to [HAA firmware](https://github.com/RavenSystem/esp-homekit-devices/wiki)

## :warning: **There is no way back to Shelly firmware if the new ZIP file has been uploaded!**
Shelly bootloader will be replaced with a standard ESP-IDF bootloader, avoiding to back to original firmware. To back to Shelly firmware or to recover it if something goes wrong, a wired connection to a PC using a FTDI adapter is needed.

:warning: **This is an third-party experimental project without any relation with Shelly or Alterco. If you decide to try it, [all is under your responsability](https://github.com/RavenSystem/mgos32toHAA/blob/main/LICENSE). :warning:**

## Requisites
- Download corresponding ZIP file from [Releases](https://github.com/RavenSystem/mgos32toHAA/releases).
- Shelly doesn't need to be updated to latest firmware version.
- Shelly doesn't need to be connected to your WiFi network.

## Instructions
1. Connect to Shelly device and open its web interface.
2. Navigate to `Settings -> Firmware`, and drag & drop the ZIP file in the firmware update area.
3. Click the `Update` button, and be sure that you don't cut power while Shelly is installing.
4. Wait until Shelly web interface tries to reload, and wair 30 seconds more to let new firmware to do the process.
5. Now, a `HAA-XXXXXX` WiFi HotSpot should be visible to start the [HAA Installation steps](https://github.com/RavenSystem/esp-homekit-devices/wiki/installation#installing-haa). Now, it is safe to cut power if you want.

Most common scripts are preloaded for several Shelly models, normally with switch functions.
