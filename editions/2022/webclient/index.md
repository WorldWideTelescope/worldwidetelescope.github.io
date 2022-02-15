---
title: 'WWT 2022 Release Notes: Web Client'
nav_exclude: true
---

# WWT 2022 Release Notes: Web Client

The WWT web client has seen substantial under-the-hood changes in WWT 2022.

## HTTPS Support

The web client now fully supports HTTPS!

## HiPS Support

The web client also now support HiPS data sets! A large number of built-in sets
are now made available in a new section of the “Explore” ribbon.

## Updated Data Collections

Beyond the new HiPS data, the web client’s [data holdings](../data/) have been
updated extensively. As of the WWT 2022 launch, they are not fully in sync with
what is exposed by the Windows client, but we expect to harmonize them in the
near future.

## User Interface for Catalog HiPS Data Sets

The new [engine](../engine/) support for progressive HiPS catalog data sets has
been wired into the user interface, so that you can click on catalogs in the
explorer and add them to the client view as layers.

## Retuned Mobile Interface

The mobile version of the webclient UI has been tuned to be a bit cleaner and
fix up a few interface elements.

## Backend Improvements

The webclient frontend has been split from the [engine](../engine/) and made
much more maintainable with release automation and continuous integration
tooling. New infrastructure also makes local testing and beta-testing much
easier (i.e., possible at all). These improvements underlie virtually all of the
fixes listed above.

## Bugfixes, etc.

Of course, the WWT 2022 webclient features many bugfixes and small improvements
not mentioned here. See the [detailed WWT 2022 components list](../components/)
for links to developer resources such as code repositories and comprehensive
changelogs.

[Go back to the WWT 2022 edition notes.](..)
