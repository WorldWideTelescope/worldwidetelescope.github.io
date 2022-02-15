---
title: 'WWT 2022 Release Notes: Windows Client'
nav_exclude: true
---

# WWT 2022 Release Notes: Windows Client

The WWT 2022 edition introduces version 6.1 of the WWT Windows client
application, with several important new features and improvements.

## Read This First

First, some disclaimers for “production” installations of WWT, such as
planetariums and kiosks:

- We are aware of [an
  issue](https://github.com/WorldWideTelescope/wwt-windows-client/issues/196) in
  which WWT will crash when used with Intel Iris Xe graphics. This appears to be
  a bug in their driver with no known workaround. Iris is an integrated graphics
  processor; if your system also has a discrete GPU, you should be able to avoid
  the crash by configuring it to use that GPU instead of Iris.
- In production scenarios, *test the new version carefully and comprehensively
  before rolling it out*. Do so in an isolated environment that cannot interfere
  with your production system. While we endeavor to keep the upgrade path as
  smooth as possible, this new version does change some under-the-hood aspects
  about the application. The core app should be as stable as ever, but it's
  always possible that some of our changes will affect some piece of your
  particular setup.
- Be aware that the WWT team provides user support on a best-effort basis. We
  aspire to provide a high level of service but *cannot* guarantee timely
  technical assistance.

If you have any questions about this, contact the team at <wwt@aas.org>.

## Installation & Getting Started

To learn more about installing and getting started with the WWT Windows client,
see the [Enthusiasts](../enthusiasts/) and [Planetarians](../planetarians/)
pages.

## HiPS Support

In tandem with the [web client](../webclient/), the WWT 2022 Windows application
adds long-awaited support for HiPS datasets! This feature was contributed by the
[China-VO] developer group. The new version includes a large built-in database
of HiPS datasets accessible in a new top-level folder in the “Explore” ribbon.
Both imagery and catalogs are supported. HiPS catalog data can be displayed to
update on-the-fly as the WWT viewport moves around on the sky.

[China-VO]: http://www.china-vo.org/

## Updated Oculus Support

The new WWT Windows application supports modern Oculus VR developer kits,
instead of the preview versions, providing compatibility with current headset
models.

## Image-Based Projector Distortion Calibration

There is early work to support calibration of dome projector distortions by
processing a captured grid display from third-party software. This functionality
is not yet documented, so reach out to <wwt@aas.org> if this capability may be
of interest to you.

## Exploring FITS Cubes

Some FITS cubes can now be loaded in the app such that you can scrub through the
cube planes interactively.

## Updated Branding and System Locations

WWT assets have been updated to align with AAS’s stewardship of the project. In
particular, installation and data storage directories are now filed under
“American Astronomical Society” rather than “Microsoft Research”. In particular:

- The default installation location has moved from `[ProgramFiles]\Microsoft
  Research\Microsoft WorldWide Telescope` to `[ProgramFiles]\American
  Astronomical Society\AAS WorldWide Telescope`.
- The user data storage location has moved from
  `[LocalAppData]\Microsoft\WorldWideTelescope` to `[LocalAppData]\American
  Astronomical Society\WorldWideTelescope`. (Here, `[LocalAppData]` is usually
  `C:\Users\[user]\AppData\Local`.)
- The location for WWT configuration registry keys has moved from
  `HKCU\Software\Microsoft\WorldWide Telescope` to `HKCU\Software\American
  Astronomical Software\WorldWide Telescope`.

These moves may break the usages of some tools such as the [Remote
Control](../remote/) or custom system startup scripts.

## More 3D Models

Now glTF 3D models (`.glb` files) can be displayed.

## “Universal Windows Platform” Framework

While we are still only distributing the standard WWT Windows application, the
WWT 6 codebase has undergone extensive revisions to prepare it for build in the
[Universal Windows Platform][uwp] (UWP), laying the groundwork for making WWT
available on a variety of different devices.

[uwp]: https://docs.microsoft.com/en-us/windows/uwp/get-started/universal-application-platform-guide

## Many More Bugfixes and Features

See the [detailed WWT 2022 components list](../components/)
for links to developer resources such as code repositories and comprehensive
changelogs.

[Go back to the WWT 2022 edition notes.](..)
