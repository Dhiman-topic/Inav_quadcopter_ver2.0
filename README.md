# Inav\_quadcopter\_ver2.0

A custom-built quadcopter with a self-designed flight controller running iNav 7.1.1, mounted on a lightweight custom aluminium frame.

Compact and powerful **STM32F411CE based flight controller** designed for **INAV firmware**.

This controller supports multiple IMU sensors and provides essential interfaces for GPS, receivers, ESCs, telemetry and peripherals.



# ⚡ Power Requirements

1. The flight controller **must be powered with a stable 5V DC supply**.

2\. Most ESCs include a **5V BEC (Battery Eliminator Circuit)** that can be used to power the flight controller.

### ⚠️ Important Warning

* The flight controller **must not be powered directly from battery voltage**.
* Only use a **stable 5V DC supply**.

Supplying incorrect voltage may **permanently damage the flight controller**.

Always verify the output voltage of your BEC before connecting it to the FC.

# ✈️ Features

* STM32F411CE MCU
* Supported IMU sensors

  * MPU9250
  * MPU6500
  * BMI160
* BMP280 Barometer
* MAX7456 OSD
* 2 Hardware UART ports
* SoftSerial support
* I2C bus for compass and peripherals
* WS2811 LED strip support
* Up to **6 motor outputs**
* Additional **servo outputs**
* Battery voltage monitoring
* Current sensing
* RSSI analog input
* Airspeed sensor input

\---

# 📦 Firmware

This flight controller runs **INAV Firmware**.

Download firmware:  inav\_xxx\_STM32F411CE.zip



`xxx` = firmware version number.

Example: inav\_7.1.1\_STM32F411CE.zip



\---

# 🖥 INAV Configurator

Download the configurator matching the firmware version.

https://github.com/iNavFlight/inav-configurator/releases

Example:

|Firmware|Configurator|
|-|-|
|INAV 7.x|Configurator 7.x|

Extract the ZIP file and run: inav-configurator.exe



\---

# 🔌 Enter DFU Mode

To flash firmware, the flight controller must be in **DFU mode**.

### Steps

1️⃣ Locate the **BOOT0 button** on the board

2️⃣ Press and **hold BOOT0**

3️⃣ Connect the USB cable to your PC

4️⃣ Release the button

If successful, **DFU** will appear in the configurator connection menu.

\---

# ⚠ DFU Driver Fix

If DFU does not appear, install drivers using:

https://impulserc.blob.core.windows.net/utilities/ImpulseRC\_Driver\_Fixer.exe

Run the program and allow it to install the required drivers.

\---

# ✅ Successful Installation

If flashing is successful:

* wait a few seconds
* the **blue LED will start blinking**

🎉 Firmware installed successfully.

\---

# ⚙ Recommended Setup Steps

After flashing firmware:

1. Calibrate accelerometer
2. Calibrate compass
3. Configure receiver
4. Configure motor outputs
5. Setup GPS (if used)
6. Setup flight modes

\---

# 🔗 Useful Links

INAV Official Website

https://inavflight.com

INAV GitHub

https://github.com/iNavFlight

INAV Documentation

https://github.com/iNavFlight/inav/wiki

\---

# 📜 License

This project is **licensed under the GNU General Public License** and is intended to support the INAV ecosystem.


\---

# ❤️ Acknowledgements

Special thanks to the **INAV community** and developers and **Rıza Çelik** for their continuous work on the firmware.





