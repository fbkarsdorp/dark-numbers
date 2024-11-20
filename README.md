# Unseen Species Models with Covariates: the case of historical criminology

The repository contains the code and data used to support the following conference paper:

Folgert Karsdorp, Mike Kestemont and Margo De Koster, "Beyond the Register: Demographic Modeling of Arrest Patterns in 1879-1880 Brussels". *Proceedings of the Conference on Computational Humanities Research 2024* ([CHR 2024](https://2024.computational-humanities-research.org/)). Denmark, Aarhus, December 4-6, 2024, CEUR-WS. ([pdf](https://ceur-ws.org/Vol-3834/paper13.pdf))

> **Abstract**: Unseen species models from ecology have recently been applied to censored historical cultural datasets to estimate unobserved populations. We extend this approach to historical criminology, analyzing the police registers of Brussels’ Amigo prison (1879-1880) using the Generalized Chao estimator. Our study aims to quantify the ‘dark number’ of unarrested perpetrators and model demographic biases in policing efforts. We investigate how factors such as age, gender, and origin influence arrest vulnerability. While all examined covariates contribute positively to our model, their small effect sizes limit the model’s predictive performance. Our findings largely align with prior historical scholarship but suggest that demographic factors alone may insufficiently explain arrest patterns. The Generalized Chao estimator modestly improves population size estimates compared to simpler models. However, our results indicate that more refined models or additional data may be necessary for robust estimates in historical criminological studies. This work contributes to the growing field of computational methods in humanities research and offers insights into the challenges of quantifying hidden populations in historical datasets.

## Data

All data is stored under the `/assets` folder:
- `amigo.xlsx`: the original, manually created data as a spreadsheet;
- `place_codes`: a spreadsheet used for the categorical mapping of birth places attested in the data set to three categories (Brussels, Belgium, or abroad).

## Software

All analyses were carried out using the notebooks in the `notebooks` folder. They should be executed in the following order:
- `preprocessing.ipynb`: takes care of preprocessing and reports some exploratory statistics;
- `analysis.ipynb`: runs the actual unseen species models.

The code was last tested using Python 3.11. All third-party dependencies can be installed via the `requirements.txt` file included in the top-level directory of this repository:

> pip install -r requirements.txt

If you want to grab the relevant version of the `copia` package (v. 0.1.5) directly from Github:

> pip install git+https://github.com/mikekestemont/copia.git@405cd6d


## Persistent archiving
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13969373.svg)](https://doi.org/10.5281/zenodo.13969373)

Releases of this repository are sustainably mirrored on [Zenodo](https://zenodo.org/), ensuring long-term archival access to this material. Please consider citing the accompanying paper if you re-use this code for academic purposes. 

## License
[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

