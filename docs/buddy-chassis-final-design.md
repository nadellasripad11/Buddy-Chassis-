# Buddy Chassis — Final Design (Week 2 CAD)

Locked 2026-10-12. Reference render: `media-generation-buddy-chassis-concept-v2-0-1dbb220c-b42a-494f-9634-5811548683a5.webp`
Cross-checked against the 33-component schematic (`buddy-robot-easyeda.json`). Nothing extra, nothing missed.

## Shell breakdown (3 printed parts)

1. **Top shell** — 3x 6mm tact button holes (SW1–SW3), speaker grille + internal speaker pocket with air cavity (J6), internal mount posts for MAX98357A module (J1), 2mm mic pinhole + mount posts for INMP441 I2S mic (Week 3 — schematic has no mic input; without it Buddy talks but can't listen)
2. **Face frame** — display window cutout (J3), translucent RGB light-pipe strip (D1)
3. **Base** — PCB standoffs (U1 + main board), 2x TT motor mounts with wheel clearance (J7/J8), battery bay, rocker switch slot (SW4), USB-C opening aligned to ESP32 (U1)

## Component cross-check (schematic → chassis)

| Des | Part | Chassis feature | Source |
|-----|------|-----------------|--------|
| U1 | ESP32-S3-DevKitC-1 | 4x M3 standoffs, USB-C opening in base | Week 1 BOM $9.99 |
| J1 | MAX98357A amp module | 2x mount posts inside top shell | Week 3 plan |
| J2 | VL53L0X ToF | **DROPPED — no window, per user 2026-10-12** | — |
| J3 | 1.47" TFT ST7789 | Window cutout in face frame | Week 1 BOM $8.99 |
| J4 | DRV8833 module | Sits on main PCB (2x10 header) | Week 1 BOM $4.99 |
| J5 | Expansion header | PCB only | ELEGOO kit |
| J6 | Speaker terminal | Speaker pocket + grille (4Ω 3W, Week 3) | Week 3 plan |
| J7/J8 | Motor terminals | 2x TT motor mounts + wire channels | Out of pocket $9–15 |
| J9 | USB_IN terminal | PCB only | Screw terminals $6.99 |
| F1 | PTC fuse | **REMOVED from BOM — footprint only, no part** | — |
| SW1–SW3 | Tact 6x6mm | 3 holes in top shell | ELEGOO kit |
| SW4 | Rocker KCD11 | Rectangular slot in base | Week 1 BOM $6.49 |
| D1 | 5mm RGB LED | Light-pipe window in face frame | ELEGOO kit |
| R1–R8, C1–C6 | Passives | PCB only | ELEGOO + cap kits |
| PWR1–3 | PWR_FLAGs | Schematic only, not physical | — |
| — | USB power bank | Bay in base, USB cable to ESP32 (decided 2026-10-12: no LiPo, no buck/TP4056) | Out of pocket $8–15 |

## Key dimensions (nominal — Amazon lists no physical sizes, verify against YOUR parts on arrival)

- ESP32-S3-DevKitC-1 (LUIRSAY clone): design for 58 x 28mm max envelope (official board ~53 x 28.5, clones run up to 58 x 28)
- 1.47" TFT module (blue PCB, 8-pin, corner mount holes): ~37–42 x 28–31mm depending on vendor; nominal cutout 40 x 30mm, active area 17.6 x 32.8mm centered
- TT gear motor: 70 x 36 x 22mm body; wheels 65mm dia — mount slots with 0.3mm clearance
- MAX98357A breakout: ~26 x 22mm
- 4Ω 3W speaker: 40mm dia pocket, 8mm deep minimum air cavity
- KCD11 rocker: 21 x 15mm panel cutout
- Tact buttons: 6x6mm, holes 6.5mm dia
- 5mm RGB LED: light pipe 6mm wide channel to face frame
- M3 standoffs: 6mm brass, PCB 4x corner holes

## Print notes

- 0.2mm layer height, 3 walls, 20% infill for shell; 40% for motor mounts
- 0.3mm clearance on all press-fit slots (motors, display)
- Print face frame face-down for a clean window edge
- Button holes: print 6.5mm, ream if tight — tact switches vary
- Design rule: every opening gets modeled from the measured part, not the nominal above
