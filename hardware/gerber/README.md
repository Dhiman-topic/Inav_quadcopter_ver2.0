# Gerber Files

Place your PCB Gerber files in this folder.

## Files to include (exported from KiCad / EasyEDA / Altium):

| File | Description |
|------|-------------|
| `*.GTL` or `*-F_Cu.gbr`   | Front copper layer |
| `*.GBL` or `*-B_Cu.gbr`   | Back copper layer  |
| `*.GTO` or `*-F_Silkscreen.gbr` | Front silkscreen |
| `*.GBO` or `*-B_Silkscreen.gbr` | Back silkscreen |
| `*.GTS` or `*-F_Mask.gbr` | Front solder mask |
| `*.GBS` or `*-B_Mask.gbr` | Back solder mask |
| `*.DRL` or `*.XLN`        | Drill file        |
| `*.GKO` or `*-Edge_Cuts.gbr` | Board outline  |

## JLCPCB Order Instructions
1. Zip all files above into `quadcopter_fc_v1.0.zip`
2. Upload the zip at [jlcpcb.com](https://jlcpcb.com)
3. Recommended settings:
   - Layers: 2
   - Thickness: 1.6mm
   - Surface finish: HASL (lead-free)
   - Silkscreen: White
   - Solder mask: Green

> ⚠️ Replace this README with your actual Gerber zip once exported from your EDA tool.
