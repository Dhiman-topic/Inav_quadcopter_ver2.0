# Build Log

## Phase 1 — Frame Design & Cutting
- Designed custom aluminium frame in CAD
- Material: 3mm 6061-T6 flat bar, 20mm wide arms
- Frame cut at local CNC shop
- Wheelbase: 450mm diagonal

## Phase 2 — FC PCB Design
- Designed custom FC in [KiCad / EasyEDA]
- MCU: STM32F405RGT6
- IMU: BMI160 (SPI)
- Baro: DPS310 (I2C)
- Ordered from JLCPCB — 5 boards, v1.0
- First board assembled and USB DFU boot confirmed

## Phase 3 — Firmware
- Flashed iNav 7.1.1
- BMI160 and DPS310 detected successfully
- GPS (M10 Ultra) locked within 90 seconds outdoors

## Phase 4 — Assembly
- Motors and ESCs mounted and soldered
- SimonK ESC calibration done (all at once via FC)
- ELRS receiver bound to transmitter (ExpressLRS 2.4GHz)
- VTX tested — clean 5.8GHz video on band 5 ch 8

## Phase 5 — First Flight
- Maiden flight in Angle mode
- Stable hover, minor yaw drift
- GPS RTH tested and working
- Flight time: ~14 minutes at 50% throttle hover

## TODO
- [ ] Tune PIDs for sport mode
- [ ] Add OSD overlay
- [ ] Test autonomous waypoint mission
- [ ] Design v1.1 FC with magnetometer onboard
