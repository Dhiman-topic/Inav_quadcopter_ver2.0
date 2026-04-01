# Tuning Notes

## Build Specs Used for Tuning
- Motors: 2212 920KV
- Props: 1045 (10 inch)
- Battery: 3S 4200mAh Li-Ion
- AUW (All Up Weight): ~850g (estimate)

## PID Values (as of v1.0)

| Axis  | P  | I  | D  |
|-------|----|----|----|
| Roll  | 40 | 30 | 15 |
| Pitch | 40 | 30 | 15 |
| Yaw   | 85 | 45 | 0  |

These are starting-point values. Tune on a calm day in Angle mode first.

## Rates
- Roll/Pitch rate: 70
- Yaw rate: 60

## Filters
- Gyro LPF: 256Hz (hardware)
- D-term LPF: default

## Known Issues / Observations
- Slight yaw wobble at hover — may need I-term increase on yaw
- GPS accuracy improves after 8+ satellite lock (wait before arming)
- Li-Ion sag noticeable below 3.3V/cell — set warning at 3.4V

## Tuning Log

| Date       | Change Made               | Result        |
|------------|---------------------------|---------------|
| 2025-01-01 | Initial flash, default PID | Flyable       |
| 2025-01-05 | P roll/pitch → 40          | Less oscillation |
