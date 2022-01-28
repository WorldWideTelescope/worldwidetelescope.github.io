---
title: 2020-08
nav_exclude: true
---

# WWT Newsletter: August 2020

Dear friends,

Welcome to the next installment of the AAS WorldWide Telescope newsletter! As
usual, a lot has been happening — but I particularly encourage you to check out
our Hubble 30-pack. It's a fantastic collection of beautiful images that you can
lose yourself in for hours!

Best,

Peter K. G. Williams
Innovation Scientist, American Astronomical Society (AAS)
Director of the AAS WorldWide Telescope Project

---

## July 2020 Content Pack: Hubble "30 for 30"

Over the month of July, we published a series of 30 classic images from Hubble
in a (slightly belated) celebration of the space telescope's 30th birthday. Each
one was nominated by an astronomer, planetarian, or other space enthusiast who
told us why they loved each image so much. As befitting a legendary telescope
like Hubble, the results were spectacular!

You should [check out the teaser video](https://www.youtube.com/watch?v=SkvlrXlhBng) and then

#### [Explore the Hubble 30 collection in the WWT web client](https://bit.ly/wwt-hst30)

For the image descriptions, see the daily forum posts presenting each image:
[thread
1](https://wwt-forum.org/t/happy-belated-30th-birthday-hubble-pictures-1-10/155/2),
[thread
2](https://wwt-forum.org/t/happy-belated-30th-birthday-hubble-pictures-11-20/165),
[thread
3](https://wwt-forum.org/t/happy-belated-30th-birthday-hubble-pictures-21-30/166).

If you want to view the collection in the Windows client or check out the data
sets "under the hood," download [the Hubble 30 WTML collection
file](https://bit.ly/wwt-hst30pack).

Special thanks to David Weigel of the US Space and Rocket Center for wrangling
nominations and data sets for this ambitious undertaking!

For August, [follow our social media
accounts](https://worldwidetelescope.org/connect/) to be notified when we
release our next content pack, all about the most magnificent planet in the
solar system: *Saturn*. For upcoming months, we're always open to suggestions!


## WWT @ IPS2020 virtual conference

Many of you might have attended the [virtual
conference](https://www.ips-planetarium.org/page/ips2020) of the [International
Planetarium Society](https://www.ips-planetarium.org/) in early August. The
American Astronomical Society was proud to help sponsor the event by presenting
a WWT video poster, produced in partnership with [Sky-Skan,
Inc](https://skyskan.com/).

#### [Check out the WWT IPS2020 video "poster"](https://youtu.be/Snhdhsq-7vQ?t=299)

If you're a planetarian interested in using WWT, either in your dome or to
connect to your audience over the web, drop us a line at <wwt@aas.org>.


## New Collaboration with Microsoft

We're excited to be able to announce a new collaboration between the WWT
development team and Microsoft. WWT has been selected to work with the Customer
Engagement Team in Microsoft's Developer Division, which specializes in helping
people that use Microsoft technologies — as WWT does, extensively — learn how to
optimize and improve their applications. In particular, WWT and Microsoft
engineers will be working together to improve the backend WWT server software
(the [wwt-website](https://github.com/worldwidetelescope/wwt-website/)
repository), which is definitely in need of a little TLC, and upgrade our
deployment mechanisms to the leading industry practices. This project won't
visibly affect your day-to-day experience with WWT, but it's part of the
never-ending work to keep WWT services running efficiently, reliably, and
securely.


## Bug Fixes and Features

The WWT software is always improving thanks to the hard work of our code-savvy
project contributors. Here are some of the improvements logged since the last
newsletter:

- [When using the web client on a Mac, rolling the view no longer pops open the Finder Scope too](https://github.com/WorldWideTelescope/wwt-web-client/pull/323)
- [When using the web client on Chrome, fix the buttons inside the Finder Scope](https://github.com/WorldWideTelescope/wwt-web-client/pull/314)
- [For developers, correctly handle data served from localhost on non-standard ports](https://github.com/WorldWideTelescope/wwt-webgl-engine/pull/52)
- [In the web client, stop eclipsed moons from disappearing if the realistic-lighting mode is off](https://github.com/WorldWideTelescope/wwt-webgl-engine/pull/56)
- [In the web client, fix panning motions when the view is rotated](https://github.com/WorldWideTelescope/wwt-webgl-engine/pull/56)
- [When using the web client on Chrome on Macs, fix occasional out-of-control zooming due to a browser bug](https://github.com/WorldWideTelescope/wwt-webgl-engine/pull/56)
- [In the web client, load certain WWT core data assets more efficiently and reliably](https://github.com/WorldWideTelescope/wwt-webgl-engine/pull/60)
- [For developers, implement a continuous integration (CI) pipeline for the Windows client codebase](https://github.com/WorldWideTelescope/wwt-windows-client/pull/161)
- [For content creators, the new version 0.3.0 of the wwt_data_formats Python package improves robustness and adds more tools for dealing with imagery data](https://github.com/WorldWideTelescope/wwt_data_formats/releases/tag/v0.3.0)


## Stay in Touch!

We always love to hear from WWT users and enthusiasts. [Follow our social media
accounts](https://worldwidetelescope.org/connect/), email <wwt@aas.org>, or post
on [the WWT forum](https://wwt-forum.org/).
