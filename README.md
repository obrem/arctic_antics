# Arctic Antics

An independently written reconstruction of **Spy vs. Spy III: Arctic Antics**, playable on a real DOS PC (8086/8088 and later, EGA/VGA or Tandy/PCjr graphics), in DOSBox, and natively on Windows, Linux and macOS.

This is an unofficial fan project. It contains **no original game files**: the installer builds your personal copy from your own copy of the original DOS game.

- **Download:** [latest release](https://github.com/obrem/arctic_antics/releases/latest)
- **Documentation:** https://obrem.github.io/arctic_antics/
- **Report a bug or ask for a feature:** [issues](https://github.com/obrem/arctic_antics/issues/new/choose)
- **What is different from the original:** [player changes](docs/changes.md)

## Quick install

There are two downloads, each a single file. Pick the version you want, or both.

| Download | Makes | Runs on |
|---|---|---|
| `Arctic-DOS-Setup` | `arctic-dos` | a real 8086/8088-or-later PC, or DOSBox |
| `Arctic-Setup` | `arctic` | Windows, macOS or Linux |

1. Put the downloaded file in the same folder as your original game files (`Spy.exe`, `Spytitle.exe`, `Spud`, `Text1.dat`, `Text2.dat`, `Text3.dat`, `Title.dat`, `Demo.dat`, `Maxx.pic`, `Trap.pic`), or in a folder directly inside it.
2. For the Tandy/AdLib music, put the C64 tape image (`SPYVSPY3.T64`) there too. Without it the game has PC speaker sound only.
3. Run the file. A few seconds later it creates the game folder next to it.

See the [installation guide](docs/install.md) for details, options and troubleshooting.

## Status

The game is playable, including the computer opponent, all tools and hazards, and both one- and two-player modes. Only the Windows package has been tested so far; the Linux and macOS packages are unverified. The DOS version is still being tuned for very slow machines. Known problems are tracked in the [issues](https://github.com/obrem/arctic_antics/issues).

## About this repository

This repository is the public home of the project: releases, documentation and issue tracking. The source code is developed privately and is not published here.

*Spy vs. Spy and Arctic Antics are the property of their respective owners. This project is not affiliated with or endorsed by them.*
