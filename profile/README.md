# Morays

_**M**imicking **O**cean **R**elevance with **A**rtificiall**Y** **I**ntelligent **S**nakes_

- [Morays](https://morays-doc.readthedocs.io/en/latest/index.html) is an organization for sharing Machine Learning-based closures for hybrid physics / AI ocean modeling. The project is intended to be ocean model agnostic with commonly agreed templates.

- It also serves as a platform for collaborative collections of examples and use cases for reproducible hybrid ocean modeling experiments.

- Ocean models taken into consideration in the Morays project are:
    - [NEMO](https://www.nemo-ocean.eu/)
    - [CROCO](https://www.croco-ocean.org/) (not started yet)


## Strategy

[Eophis](https://github.com/meom-group/eophis/) is a library that facilitates the deployment of an [OASIS](https://oasis.cerfacs.fr/en/) interface in Python scripts for coupled runs with Fortran/C geoscientific codes. This tool is particularly suitable for our purposes since an OASIS interface already exists in several ocean models.

In this context, a Morays experiment is an ocean simulation in which the physical model sends fields towards an external Python script that contains ML components. The results infered by the ML model are sent back to the ocean and retroactively used for the solution.

Newcomers are welcome to start with this [tutorial](https://morays-doc.readthedocs.io/en/latest/getting_started.html).

## Contribute

You can contribute to the use cases by creating a repository of your own experiment or add a variation of an existing experiment in the corresponding repository.

### New Experiment

- Please use the template corresponding to your code and fill it with your material as described
- An experiment is expected to be executed in the Morays framework, please read the [documentation](https://morays-doc.readthedocs.io/en/latest/index.html) to set up yours
- Potential patches and adjustments must be described in the repository


### Enrich an existing experiment

- You can add a variation of an existing experiment in the corresponding repository
- Variations must share the same software and scientific environments
