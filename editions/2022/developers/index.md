---
title: 'Get Started with WWT 2022: For Developers'
nav_exclude: true
---

# Get Started with WWT 2022: For Developers

WWT 2022 isn’t just a single application — it’s a whole toolkit for creating
rich, interactive astronomy visualization applications. If you’ve got
development skills, your imagination is the only limit!

- [Control the WWT Research App](#control-the-wwt-research-app)
- [Build a Custom WWT-Powered Web App](#build-a-custom-wwt-powered-web-app)
- [Build a WWT-Powered Desktop App in Python](#build-a-wwt-powered-desktop-app-in-python)
- [Next Steps](#next-steps)
- [Getting Help](#getting-help)


## Control the WWT Research App

You can accomplish a lot by embedding the [WWT research app][rapp] as an
`<iframe>` in a larger web app and then controlling it through its [JSON message
API][rapp-control]. This API is used by [the WWT JupyterLab extension][wwt-jlab]
to connect [pywwt] to the app.

[rapp]: https://docs.worldwidetelescope.org/research-app/latest/
[rapp-control]: https://docs.worldwidetelescope.org/research-app/latest/controlling/
[wwt-jlab]: https://github.com/WorldWideTelescope/wwt-jupyterlab
[pywwt]: https://pywwt.readthedocs.io/

To see what’s possible, [browse the API documentation][msgdocs] of the
[`@wwtelescope/research-app-messages`] NPM package, which defines the message
interface used by the app.

[msgdocs]: https://docs.worldwidetelescope.org/webgl-reference/latest/apiref/research-app-messages/
[`@wwtelescope/research-app-messages`]: https://www.npmjs.com/package/@wwtelescope/research-app-messages


## Build a Custom WWT-Powered Web App

If you need even more precise control over your web app user experience, you can
create a fully custom app built on [the WWT engine][engine-docs]. The
recommended way to do this is using [TypeScript] and the [Vue] framework with
the [Vuex] state management system. That’s how [the WWT embed][embed-src] and
the [research app][research-src] are implemented.

[engine-docs]: https://docs.worldwidetelescope.org/webgl-reference/latest/apiref/engine-vuex/
[TypeScript]: https://www.typescriptlang.org/
[Vue]: https://vuejs.org/
[Vuex]: https://vuex.vuejs.org/
[embed-src]: https://github.com/WorldWideTelescope/wwt-webgl-engine/tree/master/embed
[research-src]: https://github.com/WorldWideTelescope/wwt-webgl-engine/tree/master/research-app

The underlying WWT code is made available as a suite of NPM packages whose APIs
are documented [here][apiref]. To get a sense of how these APIs can be used,
browse the source code to [the WWT embed][embed-src] or the [research
app][research-src].

[apiref]: https://docs.worldwidetelescope.org/webgl-reference/latest/apiref/


## Build a WWT-Powered Desktop App in Python

If you’re interested in staying on the desktop, you can incorporate WWT into
Python-based [Qt] apps with [pywwt]. This interface is used by the desktop
version of [glue], for instance.

[Qt]: https://www.qt.io/
[pywwt]: https://pywwt.readthedocs.io/
[glue]: https://glueviz.org/

Check out the [`pywwt.qt` API documentation][qtapi] to see what’s possible.

[qtapi]: https://pywwt.readthedocs.io/en/stable/api/pywwt.qt.html


## Next Steps

In most cases, you’ll also want to include custom data sets in your custom WWT
apps. Never fear — plenty of data processing libraries are available as well!
The primary WWT data processing tool is the [Toasty] Python package, which is
structured as a highly modular library that can work with many kinds of data.
Underlying it is the [`wwt_data_formats`] Python package, which handles I/O on a
variety of WWT data formats.

[Toasty]: https://toasty.readthedocs.io/
[`wwt_data_formats`]: https://wwt-data-formats.readthedocs.io/

You can find the Toasty installation instructions [here][toasty-install] and
those for `wwt_data_formats` [here][wdf-install].

[toasty-install]: https://toasty.readthedocs.io/en/latest/installation.html
[wdf-install]: https://wwt-data-formats.readthedocs.io/en/latest/installation.html


## Getting Help

If you run into any issues, we recommend asking in the `#wwt` channel of the
[Astropy Slack workspace](https://astropy.slack.com/). If you're not already a
member, you can [get an Astropy Slack account](http://joinslack.astropy.org/) in
one simple step.

[Go back to the WWT 2022 edition notes.](..)
