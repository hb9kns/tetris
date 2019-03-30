# Tetris

## About

This program is a clone of the original black and white gameboy tetris, in
ascii art and in plain C. It is intended to be as similar as possible to the
original game.

## Build

`make`

Cleaning : `make clean`

## Usage

More information on program usage can be found with : `./tetris h`

To put it quickly, Esc or q quits the games, movement key are hjkl,
Return or p pause the game, m toggles music on/off.

## Features

- 1 player survival mode (game A) and challenge mode (game B).
- 2 player mode over an IP network
- Original bgm and sfx

## Notes

About key repeats : As one needs to be priviledged to access raw
keypresses and key releases, tetris is forced to work with the
system's key repeats.

About the sound : Tetris relies on oss, which has "disappeared" in
modern linux distribution. To make sound work properly, one need
to use an oss wrapper which nearly every new sound system provides.
For exemple, with aoss, in the debian package alsa-oss, simply type
`aoss ./tetris`

## Quick start

- 1 player survival mode : `./tetris`
- 2 player, on the server, with a handicap of level 4, high 3 : `./tetris 2 4 3`
- 2 player, on the client : `./tetris 2 <ip-address-of-server>:`

---

License: GPL v.3

Authors: Nicolas Carrier, Yargo Bonetti
