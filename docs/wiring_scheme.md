

## Connection Summary

```
[4200mAh Li-Ion 3S]
        │
        ├──► [4× SimonK 30A ESC] ──► [2212 920KV Motors]
        │         │ (Signal wire)
        │         └──► FC Motor Pads M1–M4
        │
        └──► [FC VBAT pad] ──► Onboard 5V BEC
                                      │
                    ┌─────────────────┼──────────────────────┐
                    │                 │                      │
              [M10 Ultra GPS]  [GEPrc ELRS RX]    [1.2W 5.8G VTX]
               UART1 TX/RX      UART2 TX/RX        5V + GND + Video
```

## Notes
- Run the video signal wire away from ESC power wires to reduce interference
- Twist VBAT and GND wires from battery to ESCs to reduce EMI
- GPS should be mounted on a mast at least 3cm above the FC for best reception
- ELRS receiver antenna should be at 90° to each other for diversity coverage
