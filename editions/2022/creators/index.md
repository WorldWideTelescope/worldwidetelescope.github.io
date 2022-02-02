---
title: 'Get Started with WWT 2022: For Image Creators'
nav_exclude: true
---

# Get Started with WWT 2022: For Image Creators

If you make your own astronomical images — whether taken directly from your own
telescope, or by processing others data — WWT 2022 offers some cool new tools
for sharing your images online. This page walks you through:

- [Install the Data Processing Tools](#install-the-data-processing-tools)
- [Try Processing Some Images](#try-processing-some-images)
- [Next Steps](#next-steps)
- [Getting Help](#getting-help)


## Install the Data Processing Tools

The WWT data processing tools are mainly provided as Python software that you
can use from the command line.

The first tool to install is [Toasty], WWT’s main image processing tool. You can
install it using either the [`pip`] tool or [`conda`] (or also [`mamba`]) if you
[activate the conda-forge package channel][cfenable]. If you're unsure, we
recommend `conda` and [conda-forge]. [Learn more about conda-forge
here][cfintro].

[Toasty]: https://toasty.readthedocs.io/
[`pip`]: https://packaging.python.org/en/latest/guides/tool-recommendations/#installation-tool-recommendations
[`conda`]: https://docs.conda.io/
[`mamba`]: https://mamba.readthedocs.io/
[cfenable]: https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge
[conda-forge]: https://conda-forge.org/
[cfintro]: https://conda-forge.org/docs/user/introduction.html

To install Toasty with [`pip`], run the following in your terminal:

```sh
pip install toasty
```

To install it with [`conda`], run:

```sh
conda install toasty
```

You might also wish to install the [WWT Aligner][aligner], a more specialized
tool. You can use the WWT Aligner to compute the sky coordinates of a bitmap
image (TIFF, JPEG, etc.) by aligning it with a one or more scientific images
(FITS) that were used to create it. The coordinates are exported as [AVM] tags,
which can be interpreted by Toasty in its [`toasty tile-study`] command.

In many cases, the amazing [Astrometry.Net][anet] service will be able to align
your image without needing a reference FITS file. But for some images,
especially those with very small fields of view, the WWT Aligner can succeed
when Astrometry.Net fails. If you might need this functionality, check out
the [WWT Aligner installation instructions][aligner-install].

[aligner]: https://docs.worldwidetelescope.org/aligner/latest/
[AVM]: https://www.virtualastronomy.org/avm_metadata.php
[`toasty tile-study`]: https://toasty.readthedocs.io/en/latest/cli/tile-study.html
[anet]: https://astrometry.net/
[aligner-install]: https://docs.worldwidetelescope.org/aligner/latest/installation/


## Try Processing Some Images

Once you have the software, you’re ready to get your data into WWT! Images need
to be specially processed for display in WWT so that they can be explored
interactively over the internet — this processing is what makes it possible for
WWT users to visualize a gigapixel-scale image without having to download, well,
a gigabyte of data.

Toasty will help you do this processing primarily through the [`toasty
tile-study`] command, which will transform a single input image. The supporting
command [`wwtdatatool preview`] will then help you preview the results to check
the alignment and appearance.

[`wwtdatatool preview`]: https://wwt-data-formats.readthedocs.io/en/latest/cli/preview.html


## Next Steps

Once you’ve processed an image, you can share it online by uploading the “tiled”
data produced by Toasty and creating a link to it using the [WWT Embed Creator
tool][embed].

[embed]: https://embed.worldwidetelescope.org/

The WWT team is hoping to build some web services that make it even easier to
upload and share your images — stay tuned!


## Getting Help

If you run into any issues, we recommend seeking support on the [WWT user
forum][forum], or asking through one of the social media channels listed on the
[Connect][connect] page.

[forum]: https://wwt-forum.org/
[connect]: https://worldwidetelescope.org/connect/

[Go back to the WWT 2022 edition notes.](..)
