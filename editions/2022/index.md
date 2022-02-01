---
title: WWT 2022
nav_exclude: true
---

# WWT 2022

The 2022 edition of AAS WorldWide Telescope will launch on February 15th, 2022.
WWT isn’t a physical telescope — it’s a suite of free and open source software
and data sets that combine to create stunning scientific visualizations and
stories. While WWT started out as a standalone Windows application, it’s evolved
into a powerful astronomy visualization toolkit that you can use on the desktop,
in the browser, and from Python. To learn more, visit [the WWT
homepage][wwthome]{:target="_blank"}.

[wwthome]: https://worldwidetelescope.org/home/

An “edition” is a coordinated release of the many software and data components
that comprise the WWT ecosystem. This edition homepage covers:

- [What’s New](#whats-new)
- [See WWT 2022 In Action](#see-wwt-2022-in-action)
- [Get Started with WWT 2022](#get-started-with-wwt-2022)


## What’s New

So many things! WWT 2022 wraps up several years’ worth of improvements to all
aspects of WWT. Highlights include:

- A new WWT “research app” for seamlessly integrated data analysis
  and visualization in [JupyterLab]
- New support for [HiPS] imagery and catalogs
- A new system for “tiling” [FITS] datasets to allow even gigapixel-scale
  scientific images to be explored interactively ([supported by the NSF][2004840])
- A dramatically expanded suite of data tools for converting all kinds of images
  and datasets into WWT’s formats (partially supported by [Space Telescope
  Science Institute][stsci])
- A new stable release of the WWT Windows application
- Literally thousands of beautiful new astronomy images integrated into WWT’s
  data holdings
- And more!

[JupyterLab]: https://jupyter.org/
[HiPS]: http://aladin.u-strasbg.fr/hips/
[FITS]: https://en.wikipedia.org/wiki/FITS
[2004840]: https://www.nsf.gov/awardsearch/showAward?AWD_ID=2004840
[stsci]: https://www.stsci.edu/

![Screenshot of WWT JupyterLab app](./jupyterlab.jpg)


## See WWT 2022 In Action

Here are some great ways to see some of the things that WWT 2022 can do:

- For researchers and other technically-minded folks, you can dive right into
  [our cloud-based tutorial notebooks][mybinder]{:target="_blank"} that
  demonstrate the usage of the new WWT JupyterLab app.
- [Click here][meerkat-gc]{:target="_blank"} to open up a freestanding version
  of the app to showcase an incredible image of the Milky Way galactic center at
  radio wavelengths from the MeerKAT telescope ([details
  here][meerkat-deets]{:target="_blank"})
- The [Solar System Explorer][sse]{:target="_blank"} is a WWT-powered
  educational web application created by the [WWT
  Ambassadors][wwta]{:target="_blank"} group. It didn’t take a team of software
  engineers to create this — just a pair of astronomer/educators with a keen eye
  for design and willingness to learn a bit of JavaScript!
- [This *Sky & Telescope* article][sandt-nye]{:target="_blank"} embeds a WWT
  “guided tour” to provide an interactive, multimedia tour of the some bright
  stars in the northern winter night sky.

[mybinder]: https://bit.ly/pywwt-notebooks
[meerkat-gc]:  https://bit.ly/wwt-meerkatgc_jan22
[meerkat-deets]: https://www.sarao.ac.za/media-releases/new-meerkat-radio-image-reveals-complex-heart-of-the-milky-way/
[sse]: http://projects.wwtambassadors.org/solar-system-explorer/
[wwta]: https://wwtambassadors.org/
[sandt-nye]: https://skyandtelescope.org/astronomy-news/tour-15-of-the-brightest-stars-on-new-years-eve-video/

All of these examples build on the WWT visualization technology that also powers
the core WWT [web client][webclient] and [Windows client][windows] applications.

[webclient]: https://worldwidetelescope.org/webclient/
[windows]: https://worldwidetelescope.org/download/

![Screenshot of WWTA Solar System Explorer app](./ssexplorer.jpg)


## Get Started with WWT 2022

There’s no one way to “install WWT” because the software spans so many different
uses. Here are our recommendations for different kinds of users:

- [Researchers](./researchers/): install WWT’s Python modules and
  Jupyter/JupyterLab extensions
- [Enthusiasts](./enthusiasts/): explore the universe with WWT's web and Windows applications
- [Educators](./educators/): explore WWT educational apps and create your own “guided tours”
- [Planetarians](./planetarians/): set up WWT in your planetarium or museum
- [Image creators](): install WWT’s data processing tools
- [App developers](): start using the WWT toolkit in Python or JavaScript/TypeScript