# mqtt-helpers

A small collection of scripts to publish stuff into [MQTT](https://mqtt.org/).

## device-tracker

An [OpenWRT](https://openwrt.org/) init script to repeatedly publish all connected devices to [MQTT](https://mqtt.org/). Not perfect, but **works for me™**.

**Setup:**
1. Move the [device-tracker](./device-tracker) to your router as `/etc/init.d/device-tracker`
2. Open the script and adjust `BROKER` and `TOPIC` to your settings
3. Install dependencies: `opkg update && opkg install mosquitto-client`
4. Enable: `/etc/init.d/device-tracker enable`
5. Start: `/etc/init.d/device-tracker start`
