---
layout: default
title: What is different from the original
---

# What is different from the original

A short list of what you will notice. Everything not listed plays like the original.

## Both versions

- Controls can be changed in ARCTIC.INI; by default white uses the arrow keys and Enter, black uses WASD and Space.
- Backspace (white) and Q (black) also open the inventory.
- Every fresh left/right press in the inventory responds at once instead of waiting for a repeat delay.
- Escape opens a pause menu with Options, Cancel and Exit; Exit goes back one step.
- Options has separate Music and Effects volume and a Snowshoes switch.
- Worn snowshoes stay on while you carry and use items; the Snowshoes option restores the original behavior.
- Snowshoes protect you from mushy snow but not from thin ice.
- Waiting in the menu starts a live demo with two computer players after 30 seconds (change or turn off with demo_idle_seconds in ARCTIC.INI), instead of the original recording.
- Game timing uses fixed clocks instead of depending on the computer's speed.
- Water chills you at a steady rate; scrolling or pushing against a wall no longer speeds it up.
- Snowballs only hit a spy in the same outdoor area.
- Sawing a hole or pouring a bucket never overwrites an item that appeared in the spot, and the bucket needs clear outdoor ground.
- A dynamite charge is used up once, and an icicle trap that hits is removed completely.
- Artwork is redrawn for EGA, Tandy/PCjr and CGA composite graphics.
- Tandy and AdLib music is derived from the C64 soundtrack, played at PAL speed and pitch, a little slower than the C64 original.
- The PC speaker plays sound effects only, without music.

## DOS version

- Graphics are detected: EGA/VGA, else Tandy/PCjr; /DISPLAY:COMPOSITE shows CGA composite colors. Plain CGA is not supported.
- Sound is detected: Tandy/PCjr, else AdLib, else the PC speaker; /AUDIO:TANDY, ADLIB or SPEAKER overrides it.
- Optional game-port joystick support, off by default: run ARCTIC /CALIBRATE once, and the stick also works in the menus.

## Windows, linux and macOS version

- The game uses EGA graphics with aspect ratio correction; Options can turn on smoother scaling.
- Gamepads work (Xbox and most others) with buttons set in ARCTIC.INI: LB/RB open the inventory, Y toggles the map, B cancels, and any button skips the intro.
- Sound uses Tandy music by default; start with --adlib or --speaker to change it.
