# Firmware — iNav 7.1.1

## Download
Get iNav 7.1.1 from the official releases:
https://github.com/iNavFlight/inav/releases/tag/7.1.1

Pick the `.hex` file matching your MCU (STM32F405 for this FC).

## Flash
1. Open [iNav Configurator](https://github.com/iNavFlight/inav-configurator/releases)
2. Connect FC via USB
3. Go to **Firmware Flasher**
4. Load the `.hex` file and click **Flash Firmware**

## Restore Configuration
1. In iNav Configurator, open the **CLI** tab
2. Copy the full contents of `inav_config/quadcopter_inav_7.1.1.diff`
3. Paste into the CLI input box and press Enter
4. Type `save` and press Enter
5. Power cycle the FC

## Notes
- Always re-calibrate the accelerometer after restoring config
- GPS baud rate is set to auto — M10 Ultra will be detected at 38400 or 115200
- VTX settings are for 5.8GHz band 5 channel 8 (Raceband R8)
