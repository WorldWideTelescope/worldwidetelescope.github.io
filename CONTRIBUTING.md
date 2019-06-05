---
title: WWT Contributors’ Guide
permalink: "/contributing/"
nav_order: 2
---

# The AAS WorldWide Telescope Contributors’ Guide

Thank you for your interest in contributing to to the AAS WorldWide Telescope!
There are many ways to contribute, and we appreciate all of them. Here are the
major sections of this guide:

* [Bug Reports](#bug-reports)
* [Pull Requests](#pull-requests)
* [Writing Documentation](#writing-documentation)

As a reminder, all contributors are expected to follow our [Code of Conduct][coc].

[coc]: ./CODE_OF_CONDUCT.md

## Stuck?

If you feel stuck and aren’t sure where to go next, you should check out the
[WWT discussion forum] at <https://wwt-forum.org/>. We aim to have a friendly
and welcoming group of WWT fans who can help you figure out the next step for
whatever you’re looking to accomplish!

[WWT discussion forum]: https://wwt-forum.org/

## Bug Reports
[bug-reports]: #bug-reports

All software has bugs, and WWT is no exception. We can’t fix what we don't
know about, so please report liberally. If you’re not sure if something is a
bug or not, feel free to file a bug anyway.

WWT is a complex software system with many pieces, so an important first step
to reporting a bug is to figure out which piece is the culprit. In our GitHub
issue tracking system, that means figuring out which Git repository is
relevant. For now, the best advice we can offer is that you consult WWT’s
[GitHub organization page](https://github.com/WorldWideTelescope/) and peruse
the list of repositories found there.

Before reporting a bug, please search existing issues in the relevant
repository as someone else may have already reported your error. This doesn't
always work, and sometimes it's hard to know what to search for, so consider
this extra credit. We won't mind if you accidentally file a duplicate report.

Similarly, to help others who encountered the bug find your issue, consider
filing an issue with a descriptive title that contains information that
might be unique to it.

Here's a template that you can use to file a bug, though it's not necessary to
use it exactly:

    <short summary of the bug>

    I tried this:

    <steps to trigger the bug>

    I expected to see this happen:

    <description>

    Instead, this happened:

    <description>

All three components are important: what you did, what you expected, what
happened instead.


## Pull Requests
[pull-requests]: #pull-requests

Pull requests are the primary mechanism we use to change WWT. GitHub itself
has some [great documentation][about-pull-requests] on using the Pull Request
feature. We use the "fork and pull" model
[described here][development-models], where contributors push changes to their
personal fork and create pull requests to bring those changes into the source
repository.

[about-pull-requests]: https://help.github.com/articles/about-pull-requests/
[development-models]: https://help.github.com/articles/about-collaborative-development-models/

Please make pull requests against the `master` branch.


## Writing Documentation
[writing-documentation]: #writing-documentation

Documentation improvements are very welcome. The WWT GitHub organization
includes many standalone repositories for various guidebook documents that are
enumerated on [the Contributor Hub main page](./index.md). Documentation pull
requests function in the same way as other pull requests.

Our documentation is written in
[Markdown](https://en.wikipedia.org/wiki/Markdown) (with the file extension
`.md`) and rendered with [Gitbook](https://www.gitbook.com/). The
documentation source structure is itself documented in the
[WWT GitBook Markdown Format Specification](https://worldwidetelescope.gitbook.io/miscellaneous/documents/gitbook-spec).


## The Fine Print to Contributing

By contributing, you agree that we may redistribute your work under the same
license used for whichever asset you’re contributing to: “CC0 1.0 Universal”
for documentation (such as this website itself), the “MIT License” for code.

Furthermore, your contributions become property of the
[.Net Foundation](https://www.dotnetfoundation.org/), which is the
organization that legally stewards ownership of the WWT project.

Finally, all contributors to the WWT are obligated to abide by the project’s
[Code of Conduct][coc]. In brief, it says that you should not be a jerk.
