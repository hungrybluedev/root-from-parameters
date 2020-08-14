# Jupyter Python notebooks for Empirical Evidence

![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/hungrybluedev/root-from-parameters?sort=semver)
![GitHub](https://img.shields.io/github/license/hungrybluedev/root-from-parameters)

## Introduction

This repository contains Jupyter notebooks (with the extension `.ipynb`) which contain the code and results bundled together into portable documents. You can view these notebooks on GitHub. They will be in read-only mode.

In order to validate the results on a local machine, refer to the [setting up](#setting-up) section.

## Description of Individual Experiments

### Comparison of theoretical and empirical PDF and CDF

[Link to the notebook](Comparison%20of%20theoretical%20and%20empirical%20PDF%20and%20CDF.ipynb)

A simulation is performed to sample values for the distribution <em>B<sup>2</sup></em> when _B_ is a uniform variate **U(0,1)**. The data obtained from the simulation is used to plot a regular frequency histogram and a cumulative frequency histogram. It is then compared against the plots of theoretical values of <em>f<sub>X</sub>(x)</em> and <em>F<sub>X</sub>(x)</em> that are calculated in the paper.

### Empirical probability of obtaining a real root

[Link to the notebook](Empirical%20Probability%20of%20obtaining%20a%20real%20root.ipynb)

A Monte Carlo simulation is performed for a range of values of the upper bound _theta_. For each _theta_, a fixed number of trials are performed. A trial is marked a success if the sampled values of _A_, _B_, and _C_ satisfy the inequality: _B<sup>2</sup>-4AC&geq;0_. The empirical probability of success is calculated for each _theta_ and compared against the theoretical value of approximately 25.4%.

## Setting up

The following instructions need to be followed to obtain a favourable development environment to be able to reproduce the results.

### Ensure Python, Pip, and Git are installed

[Python 3](https://www.python.org/downloads/) is used. Recommend version is `3.8` or higher.

Proceed to ensure that pip - the package manager for Python is installed by default.

Ensure that [Git](https://git-scm.com/) is installed.

> Subhomoy (@hungrybluedev) recommends using Windows Powershell and [Scoop](https://scoop.sh/) to install python and git on Windows:
>
> ```bash
> scoop install python git
> ```

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

## License

This work is licensed under the MIT License. Check [LICENSE](/LICENSE) for more information.

## Contact

My contact email is available in the paper. If you do not have access to that, use your preferred way of communication from the many available at my [Contact Page](https://hungrybluedev.in/contact/).
