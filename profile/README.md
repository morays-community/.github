
# Morays

_**M**imicking **O**cean **R**elevance with **A**rtificiall**Y** **I**ntelligent **S**nakes_

[![Documentation Status](https://readthedocs.org/projects/morays-doc/badge/?version=latest)](https://morays-doc.readthedocs.io/en/latest/?badge=latest)



## What is Morays organization

[Morays](https://morays-doc.readthedocs.io/en/latest/index.html) provides a collection of deployment examples of the [Eophis](https://github.com/meom-group/eophis/) package in ocean models. It also proposes a solution for sharing the model experiments across centers. Our ambition is to offer a platform for fostering exchanges amongst Eophis users.



## How Morays works

[OASIS](https://oasis.cerfacs.fr/en/) is a parallelized Fortran coupling library that performs field exchanges between coupled executables. [Eophis](https://github.com/meom-group/eophis/) is a Python library that facilitates the creation and the configuration of an [OASIS](https://oasis.cerfacs.fr/en/) interface in a Python script to couple with Fortran/C geoscientific codes. It can be deployed in any geoscientific model if it does possess an OASIS interface, which is the case of several ocean models within the climate modeling community.

In this context, a Morays experiment is an ocean simulation in which the physical model sends fields towards an external Python script deployed by Eophis. The results computed by the Python model are sent back to the ocean and retroactively used for the solution.

<img width="1118" alt="eophis_oasis_morays" src="https://github.com/user-attachments/assets/33f82493-800b-4a94-bcc1-3de653105a04">

**Typical applications include:**
- Hybrid Machine Learning (ML) / Physics modeling
- Deployment of fast evolving high-level libraries in stable low-level environment
- Prototypal code testing

Main goal of this organization is to store examples of Morays experiments for different ocean models. So far, codes taken into consideration in Morays are:
- [NEMO](https://www.nemo-ocean.eu/)
- [CROCO](https://www.croco-ocean.org/) `(not started yet)`

Every Morays experiments are documented in a self contained separate GitHub repository. List of available experiments can be found [here](https://morays-doc.readthedocs.io/en/latest/morays_exp.html).



## How to reproduce Morays experiments

Each Morays repository provides all the material for reproducing an experiment (code, model configuration, execution scripts, and post-processing for demonstration results).

- [Tutorial to reproduce experiments with NEMO](https://morays-doc.readthedocs.io/en/latest/getting_started.html) .
- `Tutoiral to reproduce experiments with CROCO (soon)`



## How to set up a Morays experiment

A Morays experiment must be considered from the Python model side, and the ocean model side.

Eophis does not intend to configure the Python side of the experiment only, but also the global coupling settings. We first encourage you to read the [Eophis documentation](https://eophis.readthedocs.io/en/latest/) to prepare the Python material.

Then, it is required to configure the ocean models in accordance with the coupling deployed by Eophis. Steps are described in Morays documentation:
- [Instructions to set up experiments with NEMO](https://morays-doc.readthedocs.io/en/latest/nemo.html)
- `Instructions to set up experiments with CROCO (soon)`



## How to contribute

You can contribute to the use cases by adding your own experiment to the Morays organization. 

Guidelines are described [here](https://morays-doc.readthedocs.io/en/latest/contribute.html).



## How to cite

To cite a Morays experiment, please use the DOI in the README of the corresponding repository.

In addition, please cite Eophis library with [![DOI](https://zenodo.org/badge/713480336.svg)](https://doi.org/10.5281/zenodo.13852038)


## License

Copyright &copy; IGE-MEOM.

Material in this organization is licensed under [BSD 3-clause and Creative Commons Attribution 4.0 International ](https://github.com/morays-community/morays-doc/blob/main/LICENSE).



## Support and bug reports

For suggestions or feature requests related to the Morays project in general, please leave an issue in this [repository](https://github.com/morays-community/.github/issues) or start a [discussion](https://github.com/orgs/morays-community/discussions).

For bug reports related to a specific experiment, please leave an issue in the corresponding repository.



## Authors and Acknowledgment

Morays is written and maintained by [IGE-MEOM group](https://github.com/meom-group).

Main contacts to this project are:

- Alexis Barge: alexis.barge@proton.me
- Julien Le Sommer: julien.lesommer@univ-grenoble-alpes.fr
