# Security Camera

A security camera using an ESP32-CAM and built with [ESPHome](https://esphome.io/).

## Install ESPHome

See [Getting Started with ESPHome](https://esphome.io/guides/getting_started_command_line.html)

```sh
pip3 install esphome
```

## Compiling and Installing

First, you must create a file `secrets.yaml` with your WiFi network and password
plus a password for your fallback hotspot password. This file should not be
checked into source control.

```yaml
wifi_ssid: "WiFi SSID"
wifi_pw: "WiFi password"
hotspot_pw: "Fallback hotspot password"
```

You can then compile and install from the command line. If you have already
programmed the device, it can be installed over the air (OTA). First time install
must be over USB.

Run the command

```sh
esphome run camera.yaml
```
