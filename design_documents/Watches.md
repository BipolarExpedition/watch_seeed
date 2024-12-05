# Starting Checklist

## Basic Setup

- [/] Add headers
- [/] Run Factory Tests
- [x] Setup IDEs
- [x] Loading basic libraries for hardware
- [/] Run Blink program

## Basic Screen Setup

- [x] Ensure all required libraries are installed (lvgl and more)
	- [x] [Getting Started with Seeed Studio Round Display for XIAO](https://wiki.seeedstudio.com/get_start_round_display/#step-3-configure-the-arduino-ide-for-the-xiao-you-are-using)
		> [!seealso]+ Additional Info
		> Information on [using LVGL and TFT](https://wiki.seeedstudio.com/using_lvgl_and_tft_on_round_display#common-interfaces-for-lvgl-library)
		> [ZIP file for latest lvgl](https://github.com/lvgl/lvgl/archive/refs/heads/master.zip)
		> 
		> Note: Libraries can also be found in Library Manager.
		
	- [x] Make sure to move the `lv_conf.h` file from `libraries/Seeed_Arduino_Round_display` is copied to `libraries`

## Battery Functions

- [/] Wire up battery
- [/] Test running on battery
- [ ] Test charging
- [ ] Test voltage measuring

> [!tip]+ Existing Measuring Technique
> For the design of the Round Display, we used the`A0`/`D0` pins on the XIAO to connect to the circuitry of the on-board battery. The remaining battery charge can be obtained by reading the analog value of this pin.

# Prototype 1

## SD Functions 1

- [ ] Detect SD
- [ ] Get a list of files
- [ ] Read a file
- [ ] Write a file

## Interaction 1

- [ ] Detect when screen is touched
- [ ] Detect position of touch
- [ ] "buttons"
- [ ] tapping

## Bluetooth Functions 1

- [ ] Scan for broadcasting devices.
- [ ] Broadcast presence
- [ ] Connect to device

## Wifi Functions 1

- [ ] Scan available networks
- [ ] Connect to network
	- [ ] Eventually use a wifi_config file for preferences, and authentications
- [] Look up a hostname
- [ ] Perform `GET` for http
- [ ] Perform `POST` for http
- [ ] Listen and receive on a socket
- [ ] Send to a socket
	

## Aesthetic Functions 1

- [ ] Customized face background (Eventually read from SD)
- [ ] Custom hands

# Links

## Hardware

[Getting Started with Seeed Studio XIAO ESP32S3 Series | Seeed Studio Wiki](https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/)
[Getting Started with Seeed Studio Round Display for XIAO | Seeed Studio Wiki](https://wiki.seeedstudio.com/get_start_round_display/)

## Software

[Arduino - ArchWiki](https://wiki.archlinux.org/title/Arduino)
[docs.arduino.cc/software/ide/#ide-v2](https://docs.arduino.cc/software/ide/#ide-v2)
[package\_esp32\_index.json](https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json)

# Specs

| Key                | Value                                |
|:----------------- | ------------------------------------ |
| Item               | Seeed Studio XIAO ESP32S3            |
| CPU Family         | ESP32-S3R8                           |
| Cpu Arch           | Xtensa LX7 dual-core, 32-bit 240 MHz |
| Wifi               | 2.4GHz                               |
| Bluetooth          | BLE: Bluetooth 5.0, Bluetooth Mesh   |
| Memory             | On-chip 8M PSRAM & 8MB Flash         |
| Low Power(s)       | 3.8V @ (25mA, 2mA, 14µA)             |
| Dimensions         | 21 x 17.8mm                          |
| Circuit Idle       | 19-22mA                              |
| Wifi Enabled Power | ~ 100mA                              |
| BLE Enabled Power  | ~ 85mA                               |
