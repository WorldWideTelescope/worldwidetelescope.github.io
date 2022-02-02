---
title: 'Get Started with WWT 2022: For Researchers'
nav_exclude: true
---

# Get Started with WWT 2022: For Researchers

For astronomy researchers and other people working with scientific astronomy
data, a great way to use WWT 2022 is in the [JupyterLab] environment. This page
walks you through:

[JupyterLab]: https://jupyter.org/

- [Try It Out Online](#try-it-out-online)
- [Install the Python Software](#install-the-python-software)
- [Next Steps](#next-steps)
- [Getting Help]

[Getting Help]: #getting-help


## Try It Out Online

To try out WWT in JupyterLab without needing to install anything, launch [our
cloud-based tutorial notebooks][mybinder]{:target="_blank"}! Because they run on
a free service ([MyBinder](https://mybinder.org/)), these notebooks lack the
computational power for many tasks, but they will give you a sense of how the
app works.

[mybinder]: https://bit.ly/pywwt-notebooks


## Install the Python Software

To use WWT 2022 on your own laptop, you should install JupyterLab and WWT’s
Python software.

If you need to install JupyterLab, [see these
instructions](https://jupyter.org/install).

For the WWT packages, you can install using either the [`pip`] tool or
[`conda`] (or also [`mamba`]) if you [activate the conda-forge
package channel][cfenable]. If you're unsure, we recommend `conda` and
[conda-forge]. [Learn more about conda-forge here][cfintro].

[`pip`]: https://packaging.python.org/en/latest/guides/tool-recommendations/#installation-tool-recommendations
[`conda`]: https://docs.conda.io/
[`mamba`]: https://mamba.readthedocs.io/
[cfenable]: https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge
[conda-forge]: https://conda-forge.org/
[cfintro]: https://conda-forge.org/docs/user/introduction.html

To install with [`pip`], run the following in your terminal:

```sh
pip install pywwt toasty wwt_jupyterlab_extension wwt_kernel_data_relay
```

To install with [`conda`], run:

```sh
conda install pywwt toasty wwt_jupyterlab_extension wwt_kernel_data_relay
```

Once that is done, there are a few extra terminal commands to help ensure that
the optimal JupyterLab experience is set up:

```sh
jupyter labextension install ipyevents @jupyter-widgets/jupyterlab-manager pywwt
jupyter nbextension install --py --sys-prefix pywwt
jupyter nbextension enable --py --sys-prefix pywwt
jupyter serverextension enable --py --sys-prefix pywwt wwt_kernel_data_relay
```

If the installation is successful, then the next time you start up JupyterLab
the “Launcher” display should now contain an AAS WorldWide Telescope icon:

![WWT JupyterLab app launcher screenshot](../jlab-launcher.jpg)

You can use this to open the WWT app, and then start controlling WWT from a
Python notebook with:

```python
from pywwt.jupyter import connect_to_app
wwt = await connect_to_app().becomes_ready()
```

The [pywwt installation instructions][pywwt-inst] contain additional information
as well as some troubleshooting steps if the above recipe doesn’t work for you.
See also [Getting Help] below.

[pywwt-inst]: https://pywwt.readthedocs.io/en/stable/installation.html


## Next Steps

Once the Python packages are installed, you should be ready to do a lot with
WWT! Once again we recommend checking out [our cloud-based tutorial
notebooks][mybinder]{:target="_blank"} to learn more about what you can do with
WWT. The [pywwt documentation][pywwt-docs] gives the detailed information about
how to control WWT from Python.

[pywwt-docs]: https://pywwt.readthedocs.io/

The WWT Python tools also install several command-line tools that you might find
useful: [`wwtdatatool`] and [`toasty`]. The [`toasty view`] command may come
especially in handy for viewing images from the command line.

[`wwtdatatool`]: https://wwt-data-formats.readthedocs.io/en/latest/
[`toasty`]: https://toasty.readthedocs.io/en/latest/
[`toasty view`]: https://toasty.readthedocs.io/en/latest/cli/view.html


## Getting Help

If you run into any issues, we recommend asking in the `#wwt` channel of the
[Astropy Slack workspace](https://astropy.slack.com/). If you're not already a
member, you can [get an Astropy Slack account](http://joinslack.astropy.org/) in
one simple step.

[Go back to the WWT 2022 edition notes.](..)
