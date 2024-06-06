# Shelly convert to HAA

This guide explains how to convert Shelly Plus, Pro and Mini (ESP32 and ESP32-C3) devices to [HAA firmware](https://github.com/RavenSystem/esp-homekit-devices/wiki)

For older Shelly devices (gen1), use this instead: [mgos to HAA Shelly ESP8266](https://github.com/RavenSystem/mgostoHAA)

[![Release](https://img.shields.io/github/v/tag/RavenSystem/mgos32toHAA?color=red&label=release)](https://github.com/RavenSystem/mgos32toHAA/releases/latest)
[![GitHub download](https://img.shields.io/github/downloads/RavenSystem/mgos32toHAA/total.svg)](https://github.com/RavenSystem/mgos32toHAA/releases/latest)
[![Donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/ravensystem)

[![Twitter](https://img.shields.io/twitter/follow/RavenSystem.svg?style=social)](https://twitter.com/RavenSystem)

[![Chat](https://img.shields.io/discord/594630635696553994?style=social)](https://discord.com/servers/esp-homekit-devices-594630635696553994)

<p align="center"><img width="300" src="https://raw.githubusercontent.com/RavenSystem/ravensystem-media/master/works-with-apple-home.svg"></p>

## :warning: **There is no OTA way back to Shelly firmware if the new ZIP file has been uploaded!**
Shelly bootloader will be replaced with a standard ESP-IDF bootloader, avoiding to back to original firmware. To back to Shelly firmware or to recover it if something goes wrong, a wired connection to a PC using a FTDI adapter is needed.

:warning: **This is a third-party experimental project, without any relation with Shelly or Alterco. If you decide to try it, [all is under your responsability](https://github.com/RavenSystem/mgos32toHAA/blob/main/LICENSE)**

#### [Source Code](https://github.com/RavenSystem/esp-homekit-devices/tree/master/HAA/HAA_mgos32_Installer)

## Pre-requisites
- Download corresponding ZIP file from [Releases](https://github.com/RavenSystem/mgos32toHAA/releases/latest).
- Shelly doesn't need to be updated to latest firmware version, but it can be updated to latest version if you want.
- Shelly doesn't need to be connected to your WiFi network, but it can be connected to your WiFi network if you want.

## Instructions [(YouTube Video with subtitles)](https://www.youtube.com/watch?v=06YHkRkwJE4)
1. Connect to Shelly device and open its web interface with a web browser using its IP address.
2. Navigate to `Settings -> Firmware`, and drag & drop or browse for the ZIP file in the `Firmware file image`.
3. Click the `Update from file` button.
4. Wait until Shelly web interface tries to reload, and wait 30 seconds more to let new firmware to do the conversion process. Be sure that you don't cut power during these 30 seconds of conversion, or your Shelly will have a chance of 1% to be bricked.
5. A `HAA-XXXXXX` WiFi HotSpot should be visible to start the [HAA Installation steps](https://github.com/RavenSystem/esp-homekit-devices/wiki/installation#installing-haa).

Most common scripts are preloaded for several Shelly models, normally with switch/button functions.

Feel free to change or modify MELPHAA script as your needs. [HAA Wiki](https://github.com/RavenSystem/esp-homekit-devices/wiki)

In addition to this firmware, you can obtain [**HAA Home Manager App**](https://github.com/RavenSystem/esp-homekit-devices/wiki/haa-home-manager), the perfect App companion
to manage your HAA devices, with batch updates, enable setup mode, and other extra features: 

<p align="center"><a href="https://apps.apple.com/app/id1556105121"><img src="https://raw.githubusercontent.com/RavenSystem/ravensystem-media/master/haamanager_app.png"></a></p>

If you want to measure the performance of your Apple Home, you can get [**Home Bench App**](https://github.com/RavenSystem/esp-homekit-devices/wiki/home-bench), the only App that performs speed tests directly over accessories using Apple HomeKit API: 

<p align="center"><a href="https://apps.apple.com/app/id6473729247"><img src="https://raw.githubusercontent.com/RavenSystem/ravensystem-media/master/homebench_app.png"></a></p>

And don't forget to subscribe to YouTube Channel:

<p align="center"><a href="https://www.youtube.com/channel/UCRumJzAoAnQ7dUpSnSUuuJw"><img width="40%" src="https://raw.githubusercontent.com/RavenSystem/ravensystem-media/master/YouTube_logo.png"></a></p>
