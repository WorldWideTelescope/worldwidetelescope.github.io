---
title: Interactive Visualization in the Age of Science Platforms
nav_exclude: true
---

# Interactive Visualization in the Age of Science Platforms: Huge FITS Images in JupyterLab with AAS WorldWide Telescope

This [ADASS32] tutorial will take place on October 31st between 19:00–21:00 UTC,
virtually.

[ADASS32]: https://www.adass2022.ca/

## For Participants: Instructions for Pre-Tutorial Preparation

If you’re going to be participating in the tutorial, you should install some
software and download some datasets in advance of the event. The following
instructions will assume familiarity with the terminal, [Git], and the
fundamentals of Python. (We will also assume a Unix-like terminal. If using
Windows, translate accordingly, or [email the presenter](#contact) for
assistance.)

[Git]: https://git-scm.com/

First, choose a location for a directory to hold tutorial-related files. The
instructions below will assume that your directory is `~/wwtviz`. If you decide
to use a different location, adjust accordingly below. This directory should be
in a place where you can create a few gigabytes of files.

1. Ensure that your directory exists. In the terminal: `mkdir -p ~/wwtviz`
1. Enter the directory in your terminal: `cd ~/wwtviz`
1. Clone the Git repository of sample WWT notebooks:
   `git clone https://github.com/WorldWideTelescope/pywwt-notebooks.git`
1. Enter the repository directory: `cd pywwt-notebooks`
1. Switch to the branch customized for this tutorial: `git checkout adass32`

For the software installation, we *strongly* recommend creating a standalone
[Conda] environment according to the following directions:

[Conda]: https://conda.io/

1. Ensure that the Conda package manager is installed on your system. If you
   don’t have it already, we recommend that you [install Conda using
   Mambaforge][install-mf]. You may need to relaunch your terminal to pick
   up necessary changes to your shell initialization files.
1. Download this file: [wwtviz.yml](./wwtviz.yml).
1. Create the environment with the command `conda env create -f wwtviz.yml`
1. Once the environment is created, it’s OK to delete the `wwtviz.yml` file.

[install-mf]: https://github.com/conda-forge/miniforge#install

To validate your software installation, try the following steps. If you run into
any problems, [email the presenter](#contact) for assistance.

1. Activate your new environment: `conda activate wwtviz`
1. Ensure JupyterLab assets are fresh: `jupyter lab build`
1. Enter sample notebooks directory: `cd ~/wwtviz/pywwt-notebooks`
1. Launch JupyterLab: `jupyter lab`
1. The JupyterLab launcher should contain a large button labeled *AAS WorldWide
   Telescope*. Clicking it should open an interactive WWT window that lets you
   navigate the sky by clicking and dragging.
1. The left-hand panel of the JupyterLab interface should contain a variety of
   sample notebooks that you can click through. The one entitled *Visualizing
   Imagery* will test out the widest range of [pywwt] functionality.
1. Close the JupyterLab window and stop the server (by typing Control-C in your
   terminal) when you’re satisfied that things are working.

[pywwt]: https://pywwt.readthedocs.io/

Next, download some larger test files that we’ll use for this tutorial:

1. Download the file [rh04475_00_01ww_tnx.fit] (729 MiB) into your
   `~/wwtviz/pywwt-notebooks` directory.
1. Download the file [HFI_SkyMap_857_2048_R2.02_full.fits] (576 MiB) into the same location.

[rh04475_00_01ww_tnx.fit]: https://data1.wwtassets.org/packages/2022/06_fits_studies/rh04475_00_01ww_tnx.fit
[HFI_SkyMap_857_2048_R2.02_full.fits]: https://irsa.ipac.caltech.edu/data/Planck/release_2/all-sky-maps/maps/HFI_SkyMap_857_2048_R2.02_full.fits

Finally, if you have any large maps that you would like to try processing at the
end of the tutorial, download or copy them as well! Here, “large” might be in
terms of either angular size, or number of pixels. If your data are spread out
over a number of FITS files, that’s OK — WWT’s tools can process FITS
collections (although they will not intelligently combine images the way
dedicated mosaicking tools such as [Montage] would).

[Montage]: http://montage.ipac.caltech.edu/


## Tutorial Description

For reference, here’s the tutorial description in the ADASS schedule:

> Astronomical data are getting bigger and bigger. They’re so big now that it’s
> completely impractical for researchers to obtain local copies of many
> important datasets, pushing us into the the age of “science platforms”:
> instead of running analysis software on local hardware, researchers do their
> work by interfacing with powerful remote systems. This paradigm shift creates
> both new opportunities and new challenges. A major challenge has to do with
> data visualization: existing astronomy data visualization tools are often
> desktop applications designed for local datasets that are small, in the sense
> that they must fit in a single computer’s memory. In the age of the science
> platform, visualization applications need to handle huge datasets, and they
> need to provide a seamless user experience when such datasets live on remote
> servers. Fortunately, we have a great software platform for building such
> applications: the web browser. Modern browsers are tools that power complex,
> interactive, network-native, multimedia applications, thanks to billions of
> dollars of industry investment. Indeed, the rise of the science platform is
> closely tied to the development of JupyterLab, a web-native framework for
> interactive computing. This tutorial will introduce participants to the tools
> and concepts that underpin modern, browser-based interactive astronomical
> visualization software, including aspects relating to the visualization user
> experience (UX) design. It will do so while working through the steps to
> visualize very large (gigapixel and beyond) FITS imagery interactively in
> JupyterLab using new features introduced in the “2022 edition” of AAS
> WorldWide Telescope (WWT) and its related tooling.


## Manual Software Environment Setup

If you’d prefer to set up your software environment without using the Conda file
given above, you’ll need an installation of Python 3.7 or newer. It will need to
have the following packages installed:

- `astropy`
- `astroquery`
- `jupyterlab` version `>=3.4`
- `pywwt` version `>=0.16`
- `reproject` version `>=0.9`
- `shapely` version `>=1.8`
- `toasty` version `>=0.18`
- `wwt_data_formats` version `>=0.16`
- `wwt_jupyterlab_extension` version `>=1.4`
- `wwt_kernel_data_relay` version `>=0.2`

After installing these packages you should confirm that you have at least the
following Jupyter server extensions installed and enabled (via `jupyter server
extension list`):

- `jupyterlab`
- `wwt_kernel_data_relay`

And the following Jupyter notebook extensions (`jupyter nbextension list`):

- `pywwt/extension`

And the following JupyterLab extensions (`jupyter labextension list`):

- `@wwtelescope/jupyterlab`
- `pywwt`

[The pywwt installation page][pywwt-install] has some more detailed instructions.

[pywwt-install]: https://pywwt.readthedocs.io/en/stable/installation.html


## Contact

Reach the workshop organizer Peter K. G. Williams at <pwilliams@cfa.harvard.edu>.