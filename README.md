# HACA 2024 - Python in an hour

This reposiitory contains code for use in the Health and Care Analytics conference 2024, in the Python in an Hour session.

The idea of this session is to give you a very brief introduction to what python can do, and some of the advantages of using python over tools like Excel.

It's designed to be run in Google Colab: <a target="_blank" href="https://colab.research.google.com/github/nhsengland/HACA-2024-python-in-an-hour/blob/main/rap_example_pipeline_python.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>
-----------

## Description

[Reproducible Analytical Pipelines](https://nhsdigital.github.io/rap-community-of-practice/) can seem quite abstract - so this repo is meant to serve as a real example, that anyone can run, to see RAP in action.

The pipeline uses artificial HES data, which was chosen as it is "like" real data used in our industry, but also freely available. 

This example pipeline uses Pandas to handle a data, a commonly used Python library, which will be installed locally in your environment when you go through the "Getting Started" steps below.

The pipeline follows three steps which are common to almost all analytical pipelines:

1. Getting the data - in this case we download the artificial HES data as a CSV which is saved into folder called 'data_in' on your machine (see the code in src/data_ingestion)
2. Processing the data - the data is processed using Pandas
3. Making outputs- the processed data is Is used to make some plots.

## Prerequisites

This code requires:

- Python (> 3.6), the official Python website has [instructions for downloading and installing python](https://wiki.python.org/moin/BeginnersGuide/Download).

## Getting Started

1. Clone the repository. To learn about what this means, and how to use Git, see the [Git guide](https://nhsdigital.github.io/rap-community-of-practice/training_resources/git/using-git-collaboratively/).

```
git clone https://github.com/nhsengland/python_colab_tutorial.git
```

2. Set up your environment, _either_ using [pip](https://pypi.org/project/pip/) or [conda](https://www.anaconda.com/). For more information on how to use virtual environments and why they are important,. see the [virtual environments guide](https://nhsdigital.github.io/rap-community-of-practice/training_resources/python/virtual-environments/why-use-virtual-environments/).

### Using pip

If you're using Windows, enter the following commands into the Command Line or Powershell:

```
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

If you're using Linux or MacOS, enter the following commands into the Terminal:

```
python -m venv .venv
source venv/bin/activate
python -m pip install -r requirements.txt
```

For Visual Studio Code it is necessary that you change your default interpreter to the virtual environment you just created .venv. To do this use the shortcut Ctrl-Shift-P, search for Python: Select interpreter and select .venv from the list.

## Licence

This codebase is released under the MIT License. This covers both the codebase and any sample code in the documentation.

Any HTML or Markdown documentation is [© Crown copyright](https://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/) and available under the terms of the [Open Government 3.0 licence](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

## Acknowledgements
- [Warren Davies](https://github.com/warren-davies4)
- [Sam Hollings](https://github.com/SamHollings)
- [Jennifer Struthers](https://github.com/jenniferstruthers1-nhs)
- [The RAP team](https://github.com/NHSDigital/rap-community-of-practice)!
