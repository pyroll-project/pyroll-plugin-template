# PyRoll Plugin

Template for PyRoll Plugin Repositories.

Please follow the following instructions when creating your own PyRoll plugins:

- The folder `pyroll` is a namespace package, place your plugin package therein to make it discoverable by the CLI for example by just renaming the nested `plugin` package to the desired).

- Use [`pytest`](https://docs.pytest.org) for creating unit tests. Place all test files in the `tests` folder.

- Update the `pyproject.toml` with your metadata. It is recommended to use [`poetry`](https://python-poetry.org) to maintain dependencies, as is preconfigured. It is recommended that the plugin major version corresponds to the PyRoll Core major version (so plugin versions 2.x.x working with `pyroll-core` 2.x.x).

- Place documentation in the `docs` folder:
    - you may provide a printable documentation using LaTeX based on the `docs.tex` template and the
      provided `PyRollDocs` class
    - you may provide a web documentation using Markdown or RST rendered by GitHub or external tools
      like [Sphinx](https://www.sphinx-doc.org)
    - you may provide a printable documentation built from Markdown or RST by tools such
      as [Pandoc](https://pandoc.org/)
    - if appropriate, include the result PDF in the commit and link it from `README.md` like [so](docs/docs.pdf)
    - include model and usage information in the documentation

- Please use a permissive license such as BSD or MIT

- Edit this readme file with contents of your own needs.
    
- If you want your plugin to be listed on the main documentation website (see [here](https://pyroll.readthedocs.io/en/latest/plugins/index.html)), please contact the maintainers preferably using an issue or PR.