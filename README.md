# Cookiecutter Conda Data Science

_A logical, reasonably standardized, but flexible project structure for doing and sharing data science work._

## Requirements

- [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html)
- [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html): This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
pip install cookiecutter
```

or

``` bash
conda install -c conda-forge cookiecutter
```

## Create a new project

In a folder where you want your project generated:

```bash
cookiecutter https://github.com/SantiagoPrietoA/cookiecutter_template
```

## Resulting directory structure

    ├── LICENSE
    ├── tasks.py           <- Invoke with commands like `notebook`.
    ├── README.md          <- The top-level README for developers using this project.
    ├── install.md         <- Detailed instructions to set up this project.
    ├── data
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    │
    │
    ├── environment.yml    <- The requirements file for reproducing the analysis environment.
    │
    │
    ├── setup.py           <- Makes project pip installable (pip install -e .)
    │                         so {{ cookiecutter.project_module_name }} can be imported.
    │
    └── {{ cookiecutter.project_module_name }}               <- Source code for use in this project.
        ├── __init__.py    <- Makes {{ cookiecutter.project_module_name }} a Python module.
        │
        ├── data           <- Scripts to download or generate data.
        │   └── make_dataset.py
        │
        │
        │
        ├── utils          <- Scripts to help with common tasks.
            └── paths.py   <- Helper functions to relative file referencing across project.
        │
        └── visualization  <- Scripts to create exploratory and results oriented visualizations.
            └── visualize.py
