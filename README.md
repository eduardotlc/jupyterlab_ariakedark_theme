# jupyterlab_ariakedark_theme

**An ariake dark palette based JupyterLab theme extension.**

|       build       |         PyPi          |
| :---------------: | :-------------------: |
| [![ci-badge]][ci] | [![pypi-badge]][pypi] |

[ci-badge]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/workflows/Build/badge.svg
[ci]: https://github.com/eduardotlc/jupyterlab_ariakedark_theme/actions/workflows/build.yml
[pypi-badge]: https://badge.fury.io/py/jupyterlab-ariakedark-theme.svg
[pypi]: https://badge.fury.io/py/jupyterlab-ariakedark-theme

eduardotcampos@usp.br [2023]

## Appearance

![Example 1](./images/jupyterlab_ariakedark_1.png)

![Example 2](./images/jupyterlab_ariakedark_2.png)

## Requirements

- JupyterLab >= 4.0.0

## Install

To install the extension, execute:

```bash
pip install jupyterlab_ariakedark_theme
```

## Uninstall

To remove the extension, execute:

```bash
pip uninstall jupyterlab_ariakedark_theme
```

## Contributing

### Development install

Note: You will need NodeJS to build the extension package.

The `jlpm` command is JupyterLab's pinned version of
[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
`yarn` or `npm` in lieu of `jlpm` below.

```bash
# Clone the repo to your local environment
# Change directory to the jupyterlab_ariakedark_theme directory
# Install package in development mode
pip install -e "."
# Link your development version of the extension with JupyterLab
jupyter labextension develop . --overwrite
# Rebuild extension Typescript source after making changes
jlpm build
```

You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.

```bash
# Watch the source directory in one terminal, automatically rebuilding when needed
jlpm watch
# Run JupyterLab in another terminal
jupyter lab
```

With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).

By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:

```bash
jupyter lab build --minimize=False
```

### Development uninstall

```bash
pip uninstall jupyterlab_ariakedark_theme
```

In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
folder is located. Then you can remove the symlink named `jupyterlab_ariakedark_theme` within that folder.

### Packaging the extension

See [RELEASE](RELEASE.md)
