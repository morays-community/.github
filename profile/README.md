# Morays

_**M**imicking **O**cean **R**elevance with **A**rtificiall**Y** **I**ntelligent **S**nakes_

[Morays](https://morays-doc.readthedocs.io/en/latest/index.html) is a project that illustrates how to deploy ML-based components in ocean models with Eophis.

It also serves as a platform for collaborative collections of ocean-models experiments conducted within this framework.

## Overview

- [Eophis](https://github.com/alexis-barge/eophis/) is a python package built on [OASIS](https://oasis.cerfacs.fr/en/) that facilitates the deployment of inference models (i.e. models based on machine learning components) for coupled runs with Earth-System simulation codes. The last OASIS version allows communication between non-homogeneously written codes. This tool is particularly suitable for our purposes since an OASIS interface already exists in several ocean models.

- Ocean models taken into consideration in the Morays project are:
    - [NEMO](https://www.nemo-ocean.eu/)
    - [CROCO](https://www.croco-ocean.org/) (not started yet)

## Contribute

You can contribute to the collections by creating a repository of your own experiment or add a variation of an existing experiment in the corresponding repository.

### New Experiment

- Please use the template corresponding to your code and fill it with your material as described
- An experiment is expected to be executed in the Morays framework, please read the [documentation](https://morays-doc.readthedocs.io/en/latest/index.html) to set up yours
- Potential patches and adjustments must be described in the repository


### Enrich an existing experiment

- You can add a variation of an existing experiment in the corresponding repository
- Variations must share the same software and scientific environments
