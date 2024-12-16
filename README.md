[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TheOpenScienceNerd/jupyter-tips/HEAD)

# Jupyter notebook tips

The materials in this repo document tips and tricks for better, cleaner and more understandable jupyter notebooks.  The teaching materials are focussed on using the Jupyter-lab IDE.

## License

The materials have been made available under an MIT license.

## Installation instructions

### Installing dependencies

All dependencies can be found in [`binder/environment.yml`]() and are pulled from conda-forge.  To run the code locally, we recommend installing [miniforge](https://github.com/conda-forge/miniforge);

> miniforge is Free and Open Source Software (FOSS) alternative to Anaconda and miniconda that uses conda-forge as the default channel for packages. It installs both conda and mamba (a drop in replacement for conda) package managers.  We recommend mamba for faster resolving of dependencies and installation of packages. 

navigating your terminal (or cmd prompt) to the directory containing the repo and issuing the following command:

```bash
mamba env create -f binder/environment.yml
```

Activate the mamba environment using the following command:

```bash
mamba activate jupyter-tips
```

Run Jupyter-lab

```
jupyter-lab
```

### Online Notebooks via Binder

The examples have been setup to run online in Jupyter notebooks via binder [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TheOpenScienceNerd/jupyter-tips/HEAD)

> mybinder.org is a free tier service.  If the repo has not been used in a while Binder will need to re-containerise the code repository, and push to BinderHub. This will take several minutes. After that the online environment will be quick to load.

## Repo overview

```
.
├── binder
│   └── environment.yml
├── CHANGES.md
├── CITATION.cff
├── LICENSE
├── notebooks
│   └── test_package.ipynb
├── pyproject.toml
├── README.md
├── tests
│   └── test_datasets.ipynb
│   └── test_model.ipynb
└── treat_sim
    ├── data
    │   └── ed_arrivals.csv
    │   └── ed_arrivals_scenario1.csv
    ├── __init__.py
    ├── datasets.py
    ├── distributions.py
    └── model.py
```

* `binder/` - contains the environment.yml file (sim) and all dependencies managed via conda, used to set-up the notebooks on Binder.
* `CHANGES.md` - changelog with record of notable changes to project between versions.
* `CITATION.cff` - citation information for the package.
* `LICENSE` - details of the MIT permissive license of this work.

