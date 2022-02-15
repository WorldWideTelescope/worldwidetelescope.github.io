---
title: 'WWT 2022 Release Notes: WWT WebGL Engine'
nav_exclude: true
---

# WWT 2022 Release Notes: WWT WebGL Engine

The “WebGL engine” is the core codebase behind all WWT-powered web applications.
It implements the WWT rendering engine in a reusable JavaScript/TypeScript
package.

## Availability as NPM Package

Historically, the WWT WebGL engine has had primitive support for reuse in
applications. In particular, one could reference `wwtsdk.js` in a `<script>` tag
and try to make do from there. WWT 2022 brings this setup into the 21st century,
now providing the engine as a reusable NPM package, [@wwtelescope/engine][npm].
You can now include WWT in JavaScript projects like any other package, opening
up the use of the entire modern web development ecosystem.

[npm]: https://npmjs.com/package/@wwtelescope/engine

## TypeScript API and Documentation

The WWT WebGL engine now also provides [TypeScript] definitions for the majority
of its API. Along with the greater reliability that comes with TypeScript, there
is now also organized [API documentation][apidocs] for many of the engine
interfaces as well. While plain JavaScript uses of the engine API still work, we
strongly recommend use of the TypeScript API.

For modern web applications powered by WWT, we recommend using the new [Vue/Vue
engine interface](../engine-vuex/) to gain a whole level of development
infrastructure above and beyond that provided by the basic engine package.

[TypeScript]: https://typescriptlang.org/
[apidocs]: https://docs.worldwidetelescope.org/webgl-reference/latest/apiref/engine/

## New Support for HiPS Datasets

In tandem with [the Windows client](../winclient/), the WWT 2022 WebGL engine
adds support for HiPS datasets and catalogs.

## New Support for Tiled FITS Datasets

WWT 2022 also adds support for rendering arbitrarily large FITS datasets using a
new “tiled” FITS data standard that follows the same semantics as WWT’s “study”
framework. This capability is not yet available in the Windows client. FITS
rendering is also now GL-accelerated if the user’s browser supports WebGL 2.

## New Support for HTTPS

The WebGL engine now fully supports HTTPS environments.

## New URL Management Framework

The engine now supports a more flexible framework for defining different kinds
of URLs and rewriting them on-the-fly. In practice, this means that it’s now
possible to beta-test updates to various built-in data files by configuring
where the engine looks for them.

## Bugfixes and Features

The WWT 2022 WebGL engine includes, many, *many*, **many** additional bugfixes
and internal improvements not mentioned here. See the [detailed WWT 2022
components list](../components/) for links to developer resources such as code
repositories and changelogs.

[Go back to the WWT 2022 edition notes.](..)
