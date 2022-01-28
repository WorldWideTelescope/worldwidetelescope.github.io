---
title: 2022-01
nav_exclude: true
---

# WWT Newsletter: January 2022

## WWT 2022 is coming: beta-test the latest version of the WWT Windows application!

Dear WWT community,

I'm excited to announce that **WWT 2022 will launch on February 15th**! This
"edition" of the WWT ecosystem gives us a chance to take stock of, and
celebrate, all of the ways that WWT has grown recently. Stay tuned for more
information about the launch event!

I'm also pleased to say that **we're entering the final beta testing period for
the new 6.1 release of the WWT Windows application!** To participate in our
"registered beta" program, visit this website:

#### <https://worldwidetelescope.org/download/beta/>

Find out more below, including some **IMPORTANT WARNINGS** to be aware of.

Best,
Peter K. G. Williams, Director of the AAS WorldWide Telescope Project

---

### WWT for Windows 6.x Final Beta Testing

The "6.x" version series of the Windows application has been in beta for a long
time, and with the WWT2022 edition we'll declare it stable. Today's beta release
(6.0.907.0) includes the first update to the core WWT data corpus in years,
adding:

- Hundreds of third-party large-area surveys made available using the
  [HiPS](http://aladin.u-strasbg.fr/hips/) format
- New huge sky maps: PanSTARRS1 3 pi, Deep Star Maps 2020, and a synthetic Gaia
  DR2 map
- Hundreds of new PR images from the European Southern Observatory, NOIRLab,
  Hubble, SOFIA, LOFAR, and more
- New Mars panoramas
- New planetary and moon maps

Big applause to WWT astrovizicist David Weigel who has prepared most of these data sets!

Download the release using the link given above ([here it is
again](https://worldwidetelescope.org/download/beta/)). We're asking for beta
users to provide their contact information so that we can provide important
updates and understand who's using the software. We'll only ever use this
information to contact you about the WWT Windows application, and you can ask us
not to contact you at all by sending a request to <wwt@aas.org>.

If you encounter any issues with the beta, please either:

- Email <wwt@aas.org> with a report, or
- [File an issue directly on
  GitHub](https://github.com/WorldWideTelescope/wwt-windows-client/issues) if
  you're comfortable with that

We don't expect to be able to fix every issue in the beta before the 6.1
release, but we hope to be able to roll out bugfixes at a regular cadence once
the 6.x series is declared stable.

Now for the **IMPORTANT WARNINGS**. If you're using WWT in a "production"
scenario, such as a planetarium or kiosk, *test the new version carefully and
comprehensively before rolling it out*. Do so in an isolated environment that
cannot interfere with your production system. While we endeavor to keep the
upgrade path as smooth as possible, this new version does change some
under-the-hood aspects about the application. The core app should be as stable
as ever, but it's always possible that some of our changes will affect some
piece of your particular use case.

We are also aware of [an
issue](https://github.com/WorldWideTelescope/wwt-windows-client/issues/196) in
which WWT will crash when used with Intel Iris Xe graphics. This appears to be a
bug in their driver with no known workaround. Iris is an integrated graphics
processor; if your system also has a discrete GPU, you should be able to avoid
the crash by configuring it to use that GPU instead of Iris. This issue is not
specific to the beta version: it also affects the 5.x series.