# EJP-RD FDP Infrastructure and VP Portal Demonstrator

This repository collects examples demonstrating how to run distributed queries to support federated analysis using the EJP-RD Virtual Platform.

To build locally you will need a version of python that is compatible with [Jupyter Book](https://jupyterbook.org/) (such as `python:3.10-slim` on Docker Hub) with the corresponding [requirements](./requirements.txt) installed (`pip install -r /path/to/requirements.txt`) to run the notebooks contained in this repository. Use the command `jupyter-book build /path/to/book`.

This repository contains an action that can build the book automatically when changes are committed to the `main` branch. If activated, the action will commit the output to a branch named `gh-pages`, that can be used with GitHub pages.
