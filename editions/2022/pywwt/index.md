---
title: 'WWT 2022 Release Notes: pywwt'
nav_exclude: true
---

# WWT 2022 Release Notes: pywwt

The [pywwt] package is the official library for interfacing with WWT from the
Python language. The WWT 2022 release of pywwt is a comprehensive update from
older versions.

[pywwt]: https://pywwt.readthedocs.io/

## Installation & Getting Started

For guidance on installing pywwt and getting started using it, see the
[Researchers](../researchers/) page.

## New Support for JupyterLab

The WWT 2022 version of pywwt provides a new way to experience WWT in
JupyterLab: in the form of the [WWT research app](../research-app/) through the
new [WWT JupyterLab extension](../jupyterlab/). While pywwt could be used in
“widget” mode before, the “app” mode is a vastly different — and superior —
experience that is only possible when using JupyterLab.

## New WWT UI

The WWT 2022 version of pywwt now has its user interface powered by the [WWT
research app](../research-app/), rather than a bare-bones custom embed of the
WWT engine. This means that many more operations can be done through the app UI
rather than requiring Python coding. This changeover may break some historical
usages of pywwt although the intention is to support old behaviors as fully as
possible.

## WWT Kernel Data Relay Now Required in Jupyter

When using pywwt in Jupyter environments, the [wwt_kernel_data_relay] Jupyter
server extension is now required. It isn’t a hard dependency of pywwt since there
are a variety of non-Jupyter cases where pywwt may be used.

[wwt_kernel_data_relay]: https://wwt-kernel-data-relay.readthedocs.io/

## New Asynchronous Support

The new release of pywwt has begun adding support for asynchronous operations
using the Python language’s built-in systems. Only a few interfaces are
supported at the moment. However, we expect more to be added as the
communication between Python and the WWT web implementation is inherently
asynchronous.

## Support for New Engine Capabilities

In WWT 2022, pywwt adds support for the major new capabilities of the [WWT WebGL
Engine](../engine/). In particular, it can load arbitrarily sized FITS datasets
by automatically tiling them with [Toasty](../toasty/). It can also load HiPS
catalogs and imagesets, with the ability to fetch data from the former.

## Bugfixes, Features, and More

The WWT 2022 release of pywwt includes a boatload of smaller bugfixes and new
capabilities. See the [detailed WWT 2022 components list](../components/) for
links to developer resources such as code repositories and comprehensive
changelogs.

[Go back to the WWT 2022 edition notes.](..)
