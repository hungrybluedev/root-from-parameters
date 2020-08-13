# Jupyter Python notebooks for Empirical Evidence

## Introduction

This repository contains Jupyter notebooks (with the extension `.ipynb`) which contain the code and results bundled together into portable documents. You can view these notebooks on GitHub. They will be in read-only mode.

In order to validate the results on a local machine, refer to the [setting up](#setting-up) section.

## Description of Individual Experiments

### 

## Setting up

The following instructions need to be followed to obtain a favourable development environment to be able to reproduce the results.

### Ensure Python, Pip, and Git are installed

Python 3 is used. Recommend version is `3.8` or higher.

Then proceed to install the Pip package manager for Python.

Ultimately, ensure that the version control system (VCS) software Git is installed.

Subhomoy (@hungrybluedev) recommends using [Scoop](https://scoop.sh/) to install python and git on Windows systems:

```bash
scoop install python git
```

On MacOS and Linux, use of the default package manager is recommend.

Pip comes preinstalled with Python (3.4 or higher).

### Setup a virtual environment for python

1. We navigate to the directory we want to store our work in.

In order to obtain the source code in this repository here are the commands necessary:

```bash
git clone https://github.com/hungrybluedev/root-from-parameters.git
```

Then `cd` into the repository:

```bash
cd root-from-parameters
```

2. We initialize a virtual environment with the command:

```bash
virtualenv statsenv
```

3. The environment is activated:

```bash
./statsenv/Scripts/activate
```

### Install required packages

```bash
pip install jupyter pandas seaborn statsmodels scipy numpy
```

This command will install the packages in the virtual environment only. It prevents interference with external projects. Packages can be updated independently without breaking the dependencies in the other projects.

### Start the Jupyter web interface

```bash
jupyter notebook
```

A web page will open in the default browser. Clicking on the required notebook will open it in a new tab where the code can be run and the results can be verified.
