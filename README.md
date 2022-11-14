# Dapla smoke tests

Notebook repo for smoke tests and feature testing of the Jupyterlab platform.

## Usage

1. Open <https://jupyter.dapla.ssb.no> or another Jupyter Lab environment
2. Clone this repo
3. Install all dependencies:

```shell
poetry install
```

4. Run the smoke tests:

```shell
poetry run poe smoke-test
```

## Prerequisites

* Python > 3.8 (3.10 is preferred)
* [Poetry](https://python-poetry.org) for dependency management
* [Poe the Poet](https://github.com/nat-n/poethepoet) for running tasks within poetry's virtualenv.
* [nbval](https://github.com/computationalmodelling/nbval) for testing and validating notebooks.

The **nbval** extension looks through every cell that contains code in an IPython notebook and then uses the **pytest** system to compare the outputs stored in the notebook with the outputs of the cells when they are executed. Because of this, the outputs of the smoke-tests are stored and not stripped (e.g. with [nbstripout](https://github.com/kynan/nbstripout)).


#### Install all dependencies

```shell
poetry install
```

## Running smoke tests

