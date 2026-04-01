# FC Pinout Reference

## Motor / ESC Signal Outputs

| Pin | Motor | Position     | Rotation    |
|-----|-------|--------------|-------------|
| M1  | ESC 1 | Rear-Right   | CW          |
| M2  | ESC 2 | Front-Right  | CCW         |
| M3  | ESC 3 | Rear-Left    | CCW         |
| M4  | ESC 4 | Front-Left   | CW          |

All ESC signal lines are 3.3V PWM at 400Hz (SimonK standard).

## UART Assignments

| UART   | Function         | Baud     |
|--------|------------------|----------|
| UART1  | ELRS / CRSF RX   | 420000   |
| UART2  | GPS (M10 Ultra)  | Auto     |
| UART3  | FPV OSD (MSP)    | 115200   |
| UART4  | Spare / Telemetry| —        |

## I2C Bus

| Address | Device  |
|---------|---------|
| 0x76    | DPS310 Barometer |

## SPI Bus

| Device  | CS Pin |
|---------|--------|
| BMI160  | PA4    |

## Power Rails

| Rail  | Source     | Used for                   |
|-------|------------|----------------------------|
| VBAT  | Battery in | ESCs, VTX (via pads)       |
| 5V    | Onboard BEC| FC logic, GPS, RX          |
| 3.3V  | STM32 LDO  | IMU, Baro, SPI/I2C devices |

## LED Indicators

| LED   | Color | Meaning                  |
|-------|-------|--------------------------|
| LED1  | Red   | Armed / Power on         |
| LED2  | Green | GPS fix acquired         |
