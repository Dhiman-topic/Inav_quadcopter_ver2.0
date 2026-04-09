# FC Pinout Reference

## Motor / ESC Signal Outputs

|Pin|Motor|Position|Rotation|
|-|-|-|-|
|M1|ESC 1|Rear-Right|CW|
|M2|ESC 2|Front-Right|CCW|
|M3|ESC 3|Rear-Left|CCW|
|M4|ESC 4|Front-Left|CW|

All ESC signal lines are 3.3V PWM at 400Hz (SimonK standard).

## UART Assignments

|UART|Function|Baud|
|-|-|-|
|UART1|GPS (M10 Ultra)||
|UART2|ELRS / CRSF RX||
|UART3|||
|||—|

## I2C Bus

|Address|Device|
|-|-|
|0x76|DPS310 Barometer|

## SPI Bus

|Device|CS Pin|
|-|-|
|BMI160|PB12|

## Power Rails

|Rail|Source|Used for|
|-|-|-|
|5V|Battery in|FC,IMU, Baro, SPI/I2C devices, GPS, RX|
||||

## LED Indicators

|LED|Color|Meaning|
|-|-|-|
|LED1 (WS2812B)|Red|Armed|
|LED2 (WS2812B)|Green BLINK|GPS fix acquired|



