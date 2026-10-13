# Journal draft — Buddy Chassis Week 2 CAD (DO NOT PUBLISH without Sripad's approval)

## Hours: 5

## Title
Week 2 CAD: Buddy chassis modeled, exported, and imported to Onshape

## Body
Designed the 3-part 3D-printed chassis for the Buddy robot as a fully
parametric CadQuery model (buddy_chassis.py — change a dimension, re-run,
get new files).

Part 1 — Base tub (160x120x40mm): 4x M3 ESP32 standoffs, 2x TT motor
plinths with shaft holes through the side walls, USB power-bank bay,
rocker-switch slot and USB-C opening in the rear wall, wire channels,
4x full-height M3 corner pillars for the lid screws.

Part 2 — Face frame: display window cutout for the 1.47" ST7789, RGB
light-pipe slot, 4x display mount posts, 2x M3 mounting holes to the
base front wall.

Part 3 — Top shell: 3x tact-button holes, speaker grille (2.5mm hole
array) over a 40mm speaker pocket with air cavity, MAX98357A mount
posts, INMP441 mic pinhole + posts, 4x corner screw holes, alignment
lip.

All parts validated (closed solids), exported as STEP + STL, and
imported into a "Buddy Chassis" Onshape document with all three parts
present.

Honest note: every fit-critical dimension is still nominal (Amazon
lists no physical sizes for the ESP32 clone, display module, or TT
motors). Each one is a named parameter at the top of buddy_chassis.py.
Nothing gets printed until the real parts are measured and the
parameters updated.

## Images (5)
1. onshape-1-assembly-iso.png — assembled view, all three parts
2. onshape-2-base-top.png — base tub, top view
3. onshape-3-angled.png — angled close view, top shell + face frame (Sripad's own screenshot)
4. onshape-4-faceframe-front.png — face frame, front view
5. onshape-5-topshell-top.png — top shell, top view
