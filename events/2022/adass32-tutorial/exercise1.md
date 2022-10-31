---
title: "Interactive Visualization Tutorial: Exercise 1"
nav_exclude: true
---

# Viz Tutorial: Exercise 1

This exercise is intended to take about 15 minutes. Please ask in the Whova chat
if you run into any problems or need any clarifications. For “big-picture”
questions, there will time for a debrief/Q&A after the exercise.


## Setup

1. Have you [installed the software and downloaded the sample data][prep] yet?
   If so, great job! If not, do that now. Ask for help in the chat if needed.
   **You won’t be able to do *anything* in this tutorial without completing the
   setup first.**
1. Open a terminal, activate your software environment, and try running the
   command `toasty`. You should get a help message about allowed subcommands.
1. Make sure that you have downloaded the file
   [vlass2.1-ql-T01t30-J145214-363000.fits] (106 MiB) into your
   `~/wwtviz/pywwt-notebooks` directory.

[prep]: ./index.md#for-participants-instructions-for-pre-tutorial-preparation
[vlass2.1-ql-T01t30-J145214-363000.fits]: https://data1.wwtassets.org/packages/2022/01_demos/vlass2.1-ql-T01t30-J145214-363000.fits


## Basic tiling

1. Open the VLASS FITS file in your favorite FITS viewer. What are its
   dimensions? Adjust the stretch (if needed) to locate the bright double radio
   galaxy, and make a mental note of its approximate position in the image.
1. The `toasty` command-line tool can break it into tiles. Run:
   ```
   toasty tile-multi-tan vlass2.1-ql-T01t30-J145214-363000.fits --hdu-index=1 --outdir=vlass
   ```
1. This will create a directory named `vlass` with one subdirectory named `4`,
   indicating a “level 4” tile grid. (“Level 0” is the top level.) How much disk
   space do the level-4 tiles consume? On most machines you can find out by
   running:
   ```
   du -hs vlass/4
   ```
1. Open the file `vlass/4/0/0_0.fits` in your favorite FITS viewer. This tile
   represents the top-left corner of the input image. Does what you see make
   sense?
1. The file name format used by Toasty in this example is
   `vlass/{L}/{Y}/{Y}_{X}.fits`. What are the `X` and `Y` values of the tile
   containing the bright double radio galaxy?


## "Cascading"

1. Now run the command that Toasty suggested earlier to generate the shallower tiles:
   ```
   toasty cascade --start 4 vlass
   ```
1. Investigate the new contents of the `vlass` directory. How much disk space
   does the entire tile pyramid consume? How does this compare to the size of
   the input image? What is the typical size of an individual tile file? (It
   will probably be faster to determine this empirically rather than
   analytically.)
1. Open the top-level tile `vlass/0/0/0_0.fits`. What is the `(x,y)` pixel
   position of the bottom-left corner of the image that actually contains data?
   What is the “efficiency” of this tiling — what percentage of this top-level
   tile actually contains data, rather than padding?

If you have extra time, try `toasty view vlass2.1-ql-T01t30-J145214-363000.fits`
to explore this image in WWT’s viewer.
