Building LaTeX with GitHub Actions
**********************************

This repository contains some experiments for testing builds of LaTeX documents using GitHub Actions.
See the runs `here <actions>`_.

Fixed:

- Operating system: ``ubuntu-20.04``.
- TeXLive version: 2019.

Variable:

- `apt.yaml <.github/workflows/apt.yaml>`_—install TeXLive using ``apt``.
- `docker.yaml <.github/workflows/docker.yaml>`_—use various Docker Hub images with TeXLive installed.
- `tinytex.yaml <.github/workflows/tinytex.yaml>`_—install TinyTeX using the `r-lib/setup-tinytex <https://github.com/r-lib/actions/tree/master/setup-tinytex>`_ action.

Observations
============

These are totally unscientific :)

- Apt run takes ~43 seconds.
- Docker run takes ~46 seconds.
- TinyTeX run takes ~65 seconds.
