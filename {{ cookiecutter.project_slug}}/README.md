# Cookiecutter Personal

A template for personal data science projects.

## Starting a new project
First you need to install cookiecutter using pip

```
$ pip install cookiecutter
```

or Conda

```
$ conda config --add channels conda-forge
$ conda install cookiecutter
```

Then run this in your terminal:

```
cookiecutter https://github.com/axlyaguana11/cookiecutter-personal
```

# Directory structure
You'll have this:

```
.
├── README.md
├── data
│   ├── processed
│   └── raw
├── environment.yml
└── notebooks
    └── 0.0-{{ cookiecutter.project_slug }}-introduction.ipynb
```