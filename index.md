---
title: WWT Contributor Hub
nav_order: 1
---

<!-- See README.md for how to preview this file when making edits -->

# Welcome to the AAS WorldWide Telescope Contributor Hub!

The [AAS](https://aas.org/)
[WorldWide Telescope](http://www.worldwidetelescope.org) (WWT) is a free,
open-source tool for visually exploring humanity’s scientific understanding of
the Universe. WWT is primarily a website that allows anyone to interactively
explore terabytes of astronomical data in a seamlessly integrated 4D
simulation of the known universe. But the WWT software ecosystem also includes
a Windows application that can power planetariums, a cloud-based web service
for discovering and sharing astronomical data, and a Python module allowing
users to write their own software to control and extend all of these systems.

WWT is brought to you by the [American Astronomical Society](https://aas.org/)
(AAS). Established in 1899 and based in Washington, DC, the AAS is the major
organization of professional astronomers in North America.

## Quick Links

- [WWT discussion forum]
- [WWT Contributors’ Guide]
- [The main WWT website!](http://www.worldwidetelescope.org/)
- [The WWT GitHub organization](https://github.com/WorldWideTelescope)
- [WWT Code of Conduct]
- [Sign up for the WWT announcements mailing list](https://bit.ly/wwt-signup)

[WWT discussion forum]: https://wwt-forum.org/

## Example Code

| Example Collection | Source Repository |
|-- | -- |
| [WWT WebGl Engine Examples] | [wwt-web-examples] |
| [“Starfield” art installation] | [wwt-kinect-swing-control] |

[WWT WebGl Engine Examples]: http://webhosted.wwt-forum.org/webengine-examples/
[“Starfield” art installation]: https://muda.co/starfield/

[wwt-web-examples]: https://github.com/WorldWideTelescope/wwt-web-examples/
[wwt-kinect-swing-control]: https://github.com/WorldWideTelescope/wwt-kinect-swing-control/

At the moment, we must host the Web examples on a separate domain that can
serve them over unsecured HTTP. This is because the core WWT web services are
not HTTPS-enabled, and so cannot be embedded inside HTTPS web pages such as
stock GitHub Pages sites. We are working to fix this!


## Stay in Touch!

Here are some ways you can communicate with the folks who make the project
happen:

- Sign up for the announcements mailing list: <https://bit.ly/wwt-signup>
- WWT discussion forum: <https://wwt-forum.org/>
- [Twitter: @wwtelescope](https://twitter.com/wwtelescope)
- [Facebook: @wwtelescope](https://www.facebook.com/wwtelescope/)
- [YouTube: AASWorldWideTelescope](https://www.youtube.com/c/AASWorldWideTelescope)
- [Email: wwt@aas.org](mailto:wwt@aas.org)


## Documentation

### Primary documents

| Document | Source Repository |
|-- | -- |
| [WWT Contributors’ Guide] | [worldwidetelescope.github.io] |
| [WWT Code of Conduct] | [worldwidetelescope.github.io] |
| [pywwt Manual and API Reference] | [pywwt] |
| [WebGL Engine Reference] | [worldwide-telescope-webgl-sdk-reference] |
| [GitBook Markdown Format Specification] | [wwtdoc-misc] |

[WWT Contributors’ Guide]: ./CONTRIBUTING.md
[WWT Code of Conduct]: ./CODE_OF_CONDUCT.md
[pywwt Manual and API Reference]: https://pywwt.readthedocs.io/
[WebGL Engine Reference]: https://worldwidetelescope.gitbook.io/webgl-engine-reference/
[GitBook Markdown Format Specification]: https://worldwidetelescope.gitbook.io/miscellaneous/documents/gitbook-spec

[worldwidetelescope.github.io]: https://github.com/WorldWideTelescope/worldwidetelescope.github.io
[pywwt]: https://github.com/WorldWideTelescope/pywwt
[worldwide-telescope-webgl-sdk-reference]: https://github.com/WorldWideTelescope/worldwide-telescope-webgl-sdk-reference
[wwtdoc-misc]: https://github.com/WorldWideTelescope/wwtdoc-misc

### Best-effort documents

Unfortunately, the following documents are not necessarily up-to-date, and may
not render correctly after
[the GitBook upgrade](https://docs.gitbook.com/v2-changes). Caveat emptor. We
aspire for all of these to be fresh, accurate, and readable, but contributor
bandwidth is limited. Contributions are more than welcome! So are GitHub
issues naming any particular sections that you would like one of the core WWT
contributors to review.

| Document | Source Repository |
|-- | -- |
| [User Manual] | [worldwide-telescope-manual] |
| [Layer Control API Reference] | [WorldWide-Telescope-Layer-Control-API] |
| [Projection Reference] | [worldwide-telescope-projection-reference] |
| [Data Tools Guide] | [worldwide-telescope-data-tools-guide] |
| [Data Files Reference] | [worldwide-telescope-data-files-reference] |
| [Pyramid SDK Reference] | [worldwide-telescope-pyramid-sdk] |
| [Advanced Guides] | [worldwide-telescope-advanced-guides] |
| [(Deprecated) HTML5 Scripting Reference] | [worldwide-telescope-web-control-script-reference] |
| [WWT Planetarium Guide] | [worldwide-telescope-planetarium] |
| [Multi-Channel Dome Guide] | [worldwide-telescope-multi-channel-dome-setup] |
| [Importing NASA SPICE Kernel Data into WorldWide Telescope] | none? |
| [Using WorldWide Telescope to produce Science Shorts] | none? |

[User Manual]: https://worldwidetelescope.gitbook.io/user-manual/
[Layer Control API Reference]: https://worldwidetelescope.gitbook.io/layer-control-reference/
[Projection Reference]: https://worldwidetelescope.gitbook.io/projection-reference/
[Data Tools Guide]: https://worldwidetelescope.gitbook.io/data-tools-guide/
[Data Files Reference]: https://worldwidetelescope.gitbook.io/data-files-reference/
[Pyramid SDK Reference]: https://worldwidetelescope.gitbook.io/pyramid-sdk-reference/
[Advanced Guides]: https://worldwidetelescope.gitbook.io/advanced-guides/
[(Deprecated) HTML5 Scripting Reference]: https://worldwidetelescope.gitbook.io/html5-control-reference/
[WWT Planetarium Guide]: https://worldwidetelescope.gitbook.io/planetarium-guide/
[Multi-Channel Dome Guide]: https://worldwidetelescope.gitbook.io/multi-channel-dome-setup/
[Importing NASA SPICE Kernel Data into WorldWide Telescope]: https://astrodavid.gitbook.io/importing-spice-kernel-data-to-worldwide-telescop/
[Using WorldWide Telescope to produce Science Shorts]: https://doctorspaceman.gitbook.io/using-worldwide-telescope-to-produce-science-shor/

[worldwide-telescope-manual]: https://github.com/WorldWideTelescope/worldwide-telescope-manual
[WorldWide-Telescope-Layer-Control-API]: https://github.com/WorldWideTelescope/WorldWide-Telescope-Layer-Control-API
[worldwide-telescope-projection-reference]: https://github.com/WorldWideTelescope/worldwide-telescope-projection-reference
[worldwide-telescope-data-tools-guide]: https://github.com/WorldWideTelescope/worldwide-telescope-data-tools-guide
[worldwide-telescope-data-files-reference]: https://github.com/WorldWideTelescope/worldwide-telescope-data-files-reference
[worldwide-telescope-pyramid-sdk]: https://github.com/WorldWideTelescope/worldwide-telescope-pyramid-sdk
[worldwide-telescope-advanced-guides]: https://github.com/WorldWideTelescope/worldwide-telescope-advanced-guides
[worldwide-telescope-web-control-script-reference]: https://github.com/WorldWideTelescope/worldwide-telescope-web-control-script-reference
[worldwide-telescope-planetarium]: https://github.com/WorldWideTelescope/worldwide-telescope-planetarium
[worldwide-telescope-multi-channel-dome-setup]: https://github.com/WorldWideTelescope/worldwide-telescope-multi-channel-dome-setup
[worldwidetelescope.github.io]: https://github.com/WorldWideTelescope/worldwidetelescope.github.io

## Get Involved

We would love your help in making WWT better! Please read the
[WWT Contributors’ Guide] and [WWT Code of Conduct] to get started. The source
code for this site lives at the [worldwidetelescope.github.io] repository.
