# WWT Contributor Hub Static Site

This repository contains the sources for the
[WWT Contributor Hub](https://worldwidetelescope.github.io/) website, served
statically via [Github Pages](https://pages.github.com/).

You might want to
[go to the WWT Contributor Hub](https://worldwidetelescope.github.io/) now:

### <https://worldwidetelescope.github.io/>


## Contributing

As you might guess, contributions to this website, and to the AAS WorldWide
Telescope in general, are welcome! See
[the contributors’ guide](https://worldwidetelescope.github.io/contributing/)
for more information (also available in this repository as
[CONTRIBUTING.md](./CONTRIBUTING.md)). We use a standard workflow with issues
and pull requests.

Our [GitHub Pages] sites, such as this one, use the [just-the-docs] [Jekyll]
theme. The [just-the-docs documentation] describes its features.

[GitHub Pages]: https://pages.github.com/
[just-the-docs]: https://github.com/pmarsceill/just-the-docs
[Jekyll]: https://jekyllrb.com/
[just-the-docs documentation]: https://pmarsceill.github.io/just-the-docs/


## Local testing

This site is based on a standard [Jekyll] static site system. As of this writing
(April 2022), Jekyll is [stuck on Ruby 2.7][ref1], while most of the rest of the
world has moved on to the Ruby 3.x series. You may need to set up and use a
custom environment with Ruby 2.7 (and C/C++ compilers for building binary gems),
e.g.:

```
conda activate ruby27
```

[ref1]: https://talk.jekyllrb.com/t/error-no-implicit-conversion-of-hash-into-integer/5890/4

Once you’ve dealt with that, run

```
bundle install
```

to make sure that the needed tools are installed, then run

```
bundle exec jekyll serve
```

to serve the site locally. For more information, see
[the GitHub documentation](https://help.github.com/en/articles/using-jekyll-as-a-static-site-generator-with-github-pages)
on Jekyll static sites.


## Acknowledgments

The AAS WorldWide Telescope system is a [.NET Foundation] project supported by
the [American Astronomical Society] (AAS) and other generous sponsors. See [the
WWT acknowledgments page][acks] to learn more.

[.NET Foundation]: https://dotnetfoundation.org/
[American Astronomical Society]: https://aas.org/
[acks]: https://worldwidetelescope.org/about/acknowledgments/
