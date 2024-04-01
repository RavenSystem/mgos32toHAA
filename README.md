# Shelly convert to HAA
This guide explains how to convert Shelly ESP32 and ESP32-C3 driven devices to [HAA firmware](https://github.com/RavenSystem/esp-homekit-devices/wiki)

## :warning: **There is no way back to Shelly firmware if the new ZIP file has been uploaded!**
Shelly bootloader will be replaced with a standard ESP-IDF bootloader, avoiding to back to original firmware. To back to Shelly firmware or to recover it if something goes wrong, a wired connection to a PC using a FTDI adapter is needed.

:warning: **This is a third-party experimental project, without any relation with Shelly or Alterco. Consider it in a BETA stage. If you decide to try it, [all is under your responsability](https://github.com/RavenSystem/mgos32toHAA/blob/main/LICENSE). :warning:**

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

Most common script is preloaded for several Shelly models, normally with switch functions.

Feel free to change or modify MELPHAA script as your needs. [HAA Wiki](https://github.com/RavenSystem/esp-homekit-devices/wiki)

In addition to this firmware, you can obtain [**HAA Home Manager App**](https://github.com/RavenSystem/esp-homekit-devices/wiki/haa-home-manager), the perfect App companion
to manage your HAA devices, with batch updates, enable setup mode, and other extra features: 

<p align="center"><a href="https://apps.apple.com/app/id1556105121"><img src="https://raw.githubusercontent.com/RavenSystem/ravensystem-media/master/haamanager_app.png"></a></p>

If you want to measure the performance of your Apple Home, you can get [**Home Bench App**](https://github.com/RavenSystem/esp-homekit-devices/wiki/home-bench), the only App that performs speed tests directly over accessories using Apple HomeKit API: 

<p align="center"><a href="https://apps.apple.com/app/id6473729247"><img src="https://raw.githubusercontent.com/RavenSystem/ravensystem-media/master/homebench_app.png"></a></p>

And don't forget to subscribe to YouTube Channel:

<p align="center"><a href="https://www.youtube.com/channel/UCRumJzAoAnQ7dUpSnSUuuJw"><img width="40%" src="https://raw.githubusercontent.com/RavenSystem/ravensystem-media/master/YouTube_logo.png"></a></p>
