---
title: "Interactive Visualization Tutorial: Exercise 2"
nav_exclude: true
---

# Viz Tutorial: Exercise 2

This exercise is intended to take about 20 minutes. Please ask in the Whova chat
if you run into any problems or need any clarifications. For “big-picture”
questions, there will time for a debrief/Q&A after the exercise.


## Setup

1. If you’re still stuck on [the setup steps][prep], keep plugging away!
1. Open a terminal and activate your software environment.
1. Change to the `~/wwtviz/pywwt-notebooks` directory.
1. Make sure that you’ve checked out the `adass32` branch of the Git
   repository.
1. If you didn’t do it before, run the command `jupyter lab build`.
   It should take a little while to complete.

[prep]: ./index.md#for-participants-instructions-for-pre-tutorial-preparation


## Basic app launching

1. Run the command `jupyter lab`. This should start up JupyterLab and open a
   browser window rooted in the demo notebooks directory.
1. Is the main view the JupyterLab “Launcher” panel? If not, use the `View →
   Activate Command Palette` menu item, then type `New Launcher` in the popup,
   then hit Enter.
1. The launcher should have a prominent button labeled “AAS WorldWide
   Telescope”. If not, ask for help in the chat. (Did you activate the
   tutorial’s software environment?)
1. Hit the button! The WWT app should load in a new panel.
1. Play around a little bit. In the “hamburger menu” at the top right of the WWT
   interface, click *Choose Background* to bring up the background chooser, and
   then try different options. You can type in the pop-up to filter the list.


## FITS visualization

1. In the “hamburger menu”, choose the *Load WTML collection* item, and paste in
   the following URL:
   `http://data1.wwtassets.org/packages/2021/09_phat_fits/index.wtml`.
1. Now choose the *Add imagery as layer* item and click on the pop-up entry box.
   There should be two options. Click on `PHAT-f475w` to load this image, which
   is derived from about 20 GiB of FITS data.
1. Change the background imagery to *PanSTARRS1 3pi*.
1. In the “Imagery” panel at the top-left of the UI, click on the line that
   reads `PHAT-f475w`. This should expand a panel with controls for adjusting
   the FITS visualization.
1. Change the stretch to *Logarithmic*.
1. Click on the “target” icon next to the row labeled *High cutoff*. Now, as you
   move your mouse around, the upper data cutoff point will change. Moving your
   mouse towards the left side of the WWT window will reduce its value; moving
   your mouse towards the right side will increase it. Moving your mouse towards
   the top edge of the window will make a bigger change; moving your mouse
   towards the bottom edge will make a smaller change. In this case, moving your
   mouse towards the **top-left** of the WWT window will have the biggest
   effect. Click your mouse button to “commit” the adjustment and exit the
   adjustment mode.
1. Do the same with the *Low cutoff* row. Instead of clicking the mouse button,
   hit the spacebar. This will “commit” the adjustment but **not** exit the
   interactive mode. To adjust one of the cutoffs by a large amount, you would
   move your mouse to the top-left or top-right corner of the WWT window and hit
   the spacebar repeatedly.
1. Move your mouse back over the line labeled `PHAT-f475w`. Click on the “eye”
   icon to hide the image. Click it repeatedly to blink the image against the
   background. Do the stars line up?
1. Play around with some of the other controls. The “map item” icon next to the
   “eye” icon returns the view to the image if you pan away from it.
1. In the *Add imagery as layer* menu, add the other PHAT image, `PHAT-f814w`.
   Tune its appearance and give it a colormap that's different than the F475W
   image. Use the opacity controls to try visualize the astrophysical colors of
   these images.


## Kernel controls

1. Open up the “NASA Exoplanet Archive” demo notebook by double-clicking on its
   row in the file explorer panel on the left edge of the JupyterLab interface.
1. Set up a side-by-side view of the WWT app and the notebook by clicking on the
   notebook’s tab and dragging it to the middle-left edge of the main JupyterLab
   work area. A blue rectangle should preview the layout that you’ll get.
1. Work through the notebook tutorial! After you “connect” the notebook to the
   WWT app, the app’s background will change due to some legacy-preserving
   behavior in pywwt. Run the code `wwt.foreground_opacity = 0` in a new cell in
   order to keep the pywwt and the app more in sync.

If you have more time, check out some of the other sample notebooks! The *Data
Gallery* collection includes a variety of other large FITS images that you can
play with.

You can also [go back to the tutorial landing page](./index.md).