---
title: 'WWT 2022 Release Notes: Aligner'
nav_exclude: true
---

# WWT 2022 Release Notes: Aligner

WWT 2022 marks the first release of the WWT Aligner app, which is intended to
help assign correct astrometric information to press-release imagery.

In particular, the aligner addresses a fairly specific problem. Say that you
have an astronomical image in an RGB format (e.g., TIFF or JPEG). If it's
missing astrometric referencing information and you want to change that, the
amazing [Astrometry.Net][anet] service can often figure out the positioning just
from the stars in your image, without any external help at all. But in some
situations, such as when an image has a very small field of view, Astrometry.Net
might fail.

[anet]: https://astrometry.net/

In these cases, the WWT Aligner might be of assistance. If you can provide it
with both your image and one or more FITS files from which the image data
originated, it will try to align the two and transfer coordinate information
from the FITS data. Under the hood, this is actually done using the
Astrometry.Net software — the Aligner generates custom “indexes” from the FITS
data that can be fed into its solver algorithm.

## Installation

For guidance on installing the WWT Aligner and getting started using it, see the
[Image Creators](../creators/) page.

For more information, see [the WWT Aligner documentation][docs]. See the
[detailed WWT 2022 components list](../components/) for links to developer
resources such as code repositories and changelogs.

[docs]: https://docs.worldwidetelescope.org/aligner/latest/


[Go back to the WWT 2022 edition notes.](..)
