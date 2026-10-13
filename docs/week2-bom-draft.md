# Buddy Week 2 — Half Life BOM draft (Tier 1, $30 cap)

Prepared 2026-10-13, revised with Sripad's "do what you think is good" (2026-10-13).
Paste-ready rows for the Half Life Week 2 BOM form.
All prices are the checkout prices you will pay; Half Life counts tax + shipping inside the $30 tier.

## Decision: motors + M3 screw set (Sripad: "add the screw set M3", 2026-10-13)

M3 moves from the Week 5 keyboard BOM into Week 2. Week 5 keeps the USB power bank only.

| # | Part | Qty | Vendor | Link | Price | Purpose (for the Half Life row) |
|---|------|-----|--------|------|-------|----------------------------------|
| 1 | HALJIA 2Pcs DC Drive Gear Motor Dual Shaft + Tire Wheel (3V-6V, 65mm wheels) | 1 pack (2 motors + 2 wheels) | haljia.com | https://www.haljia.com/products/haljia-2pcs-dc-drive-gear-motor-dual-shaft-and-tire-wheel-for-dc-3v-6v-smart-car-robot-projects-compatible-with-arduino?variant=42226972557558 | $7.99 | Drives the 2x TT motor mounts (J7/J8) modeled into the chassis base; mounts cannot be verified without the motors |
| 2 | M3 brass standoff + screw + nut assortment kit (120pcs) | 1 kit | haljia.com (cheapest verified M3 kit; confirm Amazon checkout price) | — | $9.99 | 4x M3 standoffs for ESP32, 4x lid screws into corner pillars, 2x face-frame screws, display posts |

Pre-tax total: **$17.98**. After ~8% tax: **~$19.42**. Headroom: **~$10.58** under the $30 Tier 1.

## Consequences

- Print service no longer fits: motors + M3 + print service (~$15-25) would land around $37-45 after tax, over Tier 1. Printing is NOT required for Week 2 (verified from the draft requirements), so the chassis stays digital this week. If a school printer is available, that's free and outside the BOM.
- Week 5 keyboard BOM now needs only the USB power bank for Buddy parts (M3 fulfilled here). The buddy-week5-battery-reminder was updated accordingly.
- Wires: not needed. The Week 1 ELEGOO kit already includes jumper wires.
- Filament: not needed. Sripad has no 3D printer.
- PLA+ upgrade: skipped, plainly over budget with M3 in.

## Why not the other options

- M3 kit was originally slated for Week 5's keyboard build — moved here per Sripad 2026-10-13; Week 5 no longer needs it.

## Notes

- You buy these yourself: Amazon blocks my browser, so I cannot verify Amazon-side listings or prices. The two brand-store links above are the verified price anchors from last night's check; on your Amazon rows, search the exact product names and use your checkout prices. If an Amazon equivalent costs more than the anchor, redo the math above.
- Prefer Prime-eligible Amazon listings: shipping counts inside the tier, so $0 shipping matters.
- If you already have a spool of black PLA, drop row 2 and you are at ~$14 before tax, comfortably under.
- Still yours to do for the Oct 18, 11:59 PM close: repo link, cover image (your Onshape screenshots in this workspace are the real-image candidates), Hackatime link, and saying the word on the progress reel.
