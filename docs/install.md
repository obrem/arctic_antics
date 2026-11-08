---
layout: default
title: Installation
---

# Installation

## What you need

- The **original DOS Spy vs. Spy III: Arctic Antics** files. The installer reads them once and builds your personal data from them; nothing is uploaded and no original file is changed.
- Optional, for Tandy/AdLib music: the **C64 tape image** (`SPYVSPY3.T64`) of the same game. Without it the game still installs and plays with PC speaker sound.

Required original files (names are matched without regard to case): `Spy.exe`, `Spytitle.exe`, `Spud`, `Text1.dat`, `Text2.dat`, `Text3.dat`, `Title.dat`, `Demo.dat`, `Maxx.pic`, `Trap.pic`.

## Choose a download

Each download is **one file**. The setup program contains only this project's own work (the setup program, the game, licence notices and sealed art and music bundles). It contains no original game files.

| Download | Makes | Runs on |
|---|---|---|
| `Arctic-DOS-Setup.exe` | `arctic-dos` | a real 8086/8088-or-later PC, or DOSBox: `ARCTIC.EXE` |
| `Arctic-Setup.exe` | `arctic` | Windows: `Arctic Antics.exe`. Linux and macOS: `arctic-sdl` |

Verify a download against the `.sha256` file on the release page if you like.

## Install

1. Put the downloaded file in the **same folder as your original files**, or in a folder directly inside that folder. It looks nowhere else (not the parent folder, not Downloads). If files are missing it stops with an error naming them; you can also point it at them with `--originals <folder>`.
2. For Tandy/AdLib music, put `SPYVSPY3.T64` in the same place (or give `--c64 <file>`).
3. Run the file: double-click it, or run `Arctic-Setup install` from a terminal. On Linux and macOS the download is a `.tar.gz` holding the one file; extract it first.
4. In a few seconds it creates the game folder (`arctic-dos` or `arctic`) next to the installer, holding the program, the data files, `ARCTIC.INI` (controls and options), a short README and `CHANGES.TXT`. The setup file is no longer needed afterwards.

The data files are compiled from your originals on your computer, so keep them private. Running the installer again replaces the data and keeps your edited `ARCTIC.INI`.

Installer options: `--originals <folder>`, `--output <folder>`, `--c64 <tape image>`, `--cache <folder>` (keep the editable artwork cache), `--yes` (never ask questions).

## Playing

- White spy: arrow keys, **Enter** to pick up and use. Black spy (two players): **W A S D**, **Space**. Escape opens the pause menu. All keys can be changed in `ARCTIC.INI`.
- Windows, Linux and macOS: gamepads work (Xbox and most others).
- DOS: sound and graphics are detected automatically. Override with `/DISPLAY:` and `/AUDIO:` switches, for example `ARCTIC /AUDIO:ADLIB` or `ARCTIC /DISPLAY:COMPOSITE`. Optional game-port joystick support is off by default; run `ARCTIC /CALIBRATE` once to set it up.

See [what is different from the original](changes.html) for the full list.

## DOS requirements

- DOS 3 or later, an 8086/8088 or later processor, and 640 KB of memory.
- EGA/VGA graphics, or Tandy/PCjr graphics. Plain CGA is not supported; CGA composite colours are available with `/DISPLAY:COMPOSITE`.
- A PCjr additionally needs 640 KB expanded memory.
- AdLib sound needs an OPL2-compatible card at ports 388h/389h.
- DOSBox is fine. A higher CPU cycle setting is smoother; very slow machines are still being tuned.

## Troubleshooting

- **"Files missing" error:** the installer lists them. Check that the files are in the same folder as the installer, or give `--originals <folder>`.
- **No Tandy/AdLib music:** the C64 tape image was not found. Put `SPYVSPY3.T64` next to the installer and run it again.
- **Windows warns about an unknown publisher:** the downloads are not code-signed.

If something else goes wrong, please [open an issue](https://github.com/obrem/arctic_antics/issues/new/choose) with your platform, the setup file you used and what the installer printed. Please do not attach original game files or the `.DAT` data files.
