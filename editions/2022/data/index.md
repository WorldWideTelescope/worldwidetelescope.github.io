---
title: 'WWT 2022 Release Notes: Data Holdings'
nav_exclude: true
---

# WWT 2022 Release Notes: Data Holdings

WWT 2022 includes a massive increase in the data holdings that constitute the
core WWT corpus.

## New HiPS Datasets

The most noteworthy change to WWT’s data holdings for WWT 2022 is the addition
of hundreds of HiPS surveys and catalogs. For backwards-compatibility reasons,
these are indexed in their own folder of “HiPS” or “External” surveys in the
Explore menus of the WWT client applications. These datasets are generously made
available by our European partners, and due to the nature of the HiPS format
they may load somewhat more slowly than datasets from WWT’s servers.

## Merged “VAMP” Feeds

For a while now, the WWT web client has included a "Latest Imagery" collection
populated with image feeds from WISE, Chandra, Hubble, Spitzer, and ESO made
available as part of the [VAMP] project and [AstroPix]. While WWT’s update
mechanism for these feeds has been inoperative for a few years now, they still
contain hundreds of new images that were not straightforwardly accessible in the
Windows client. These feeds have now been integrated into data corpus accessible
to the Windows client.

[VAMP]: https://www.virtualastronomy.org/
[AstroPix]: https://astropix.ipac.caltech.edu/

## New All-Sky Maps

New all-sky maps available in WWT 2022 include [Gaia DR2][gdr2], [PanSTARRS1
3pi][ps3pi], and the [Deep Star Maps 2020][dsm2020].

[gdr2]: https://www.cosmos.esa.int/web/gaia/dr2
[ps3pi]: https://panstarrs.stsci.edu/
[dsm2020]: https://svs.gsfc.nasa.gov/4851

## New And Updated Observatory Collections

WWT astrovizicist David Weigel has imported hundreds of new images provided by
NOIRLab and the European Southern Observatory. These have been merged with the
pre-existing NOAO collection and the ESO VAMP feed, respectively.

Smaller collection updates include WISE, SOFIA, LOFAR, and Hubble.

## New Planet Maps

David also imported many new planetary maps from recent missions like Cassini
and New Horizons, including:

- Mimas
- Enceladus
- Tethys
- Dione
- Rhea
- Titan
- Iapetus
- Phoebe
- Ceres
- Bennu
- THEMIS Infrared Mars map

## New Panoramas

David also imported several new Mars panoramas from Perseverance and Curiosity,
as well as some previously-unavailable Apollo panoramas and a special image
entitled “North Meets South” produced by ESO.

## Fixed Spitzer URLs

The URLs associated with images in the Spitzer collection were broken by updates
to the Spitzer web presence. These have been fixed to the extent possible.

## Cleanups

Some images with bad astrometry have been removed, including several redundant
images of the Crab nebula. A variety of pieces of metadata have been fixed up.

## New Data Holdings Database

To create the WWT 2022 data update, we organized the existing WWT data holdings
into a common database that is now version-controlled on GitHub in a repository
named [wwt-core-catalogs]. The repository comes with a management script that
automates the creation and maintenance of the WTML files that define the corpus.
This new piece of infrastructure will massively ease future data updates, which
we expect to occur much more frequently going forward.

[wwt-core-catalogs]: https://github.com/WorldWideTelescope/wwt-core-catalogs

[Go back to the WWT 2022 edition notes.](..)
