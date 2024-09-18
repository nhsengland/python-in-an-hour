# Python in an hour

This repo will give you a very brief introduction to what Python can do for you as someone who works with data, and some of the advantages of using Python over tools like Excel.

We have two notebooks in here - one to show some basic data processing, and one to show a visualisation tool called D-Tale.

You can run this code in GitHub Codespaces, locally on any machine with Python installed (see instructions below), or with Google Colab at these links: 

Data processing notebook: <a target="_blank" href="https://colab.research.google.com/github/nhsengland/python-in-an-hour/blob/main/rap_example_pipeline_python.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

D-Tale notebook: <a target="_blank" href="https://colab.research.google.com/github/nhsengland/python-in-an-hour/blob/main/Visualising_data_with_dtale.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>


-----------

## RAP Example Pipeline

The rap_example_pipeline_python.ipynb notebook, demonstrates - in a very simple way - the three main steps common to almost all analytical processes:

1. **Get the data** - in this case we'll download the artificial HES data from the web
2. **Process the data** - we'll do a simple aggregation
3. **Making outputs** - we'll make some charts

### The data we'll use

We'll use the artificial Hospital Episode Statistics (HES) data. This has the same structure as the real HES used in our industry, but it's mock data - there's no personally identifiable information in it. 

### Packages

One of the great advantages of Python is that you can use other people's code in your projects. This can save you a lot of time!

How this works is like this:

1. Someone writes some useful Python code
2. They think, "Hey this would be really useful, I want to share this with the world!"
3. They turn their code into something called a "package"
4. They upload their package to a central package repository called PyPi
5. You install their package from PyPi and use their code in your project!

### Pandas

In this demo, we'll use a package called `Pandas`.

Pandas can do pretty much anything you can do with other tools like Excel and SQL. You can filter, group, create aggregations, make pivot tables, and, in combination with other packages, even make charts!

It's one of the most commonly-used packages by data analysts.

### Running the code

Simply load up the rap_example_pipeline_python.ipynb notebook in Codespaces, Google Colab, or in your local environment if you know how to set this up, and follow the instructions inside!

## Visualising data with D-Tale

The Visualising_data_with_dtale.ipynb file showcases a Python package called D-Tale, which you can use to visualise and explore datasets. This notebook loads up some publically available Covid data into D-Tale, so that you can play around with it's features.

With just a few lines of code you'll get a GUI interface, from where you can process data, create charts, and perform various kinds of analysis in a few clicks.

One useful feature of this package is that when you do something with it, such as change a data type of a column or create a chart, it can display the Python code it used to carry out that function. So it's a pretty handy learning tool as well as a nice way to explore data.

### Running the code

As with the example pipeline notebook, just load up the Visualising_data_with_dtale.ipynb file and click Run All. D-Tale should open in a new window.

### Things to try

Try having a look around the D-Tale interface and see what you can do with it. You might try for example...

1. The date column appears to have been imported as a string. Can you convert it to a date type? (hint: click the column name at the top for some transformations you can do)
2. Could you find a way to group the data by country and count the number of covid cases?
3. Once you have done step 2, could you use this aggregate data and make a bar chart out of it?

Keep an eye out for the `<>` icons - if you click these, D-Tale will display the Python code it's using under the bonnet!

## Prerequisites

This code requires:

- Python (> 3.6), the official Python website has [instructions for downloading and installing python](https://wiki.python.org/moin/BeginnersGuide/Download).

## Getting Started

### Running locally

1. Clone the repository. To learn about what this means, and how to use Git, see the [Git guide](https://nhsdigital.github.io/rap-community-of-practice/training_resources/git/using-git-collaboratively/).

```
git clone https://github.com/nhsengland/python_colab_tutorial.git
```

2. Set up your environment.

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

For more information on how to use virtual environments and why they are important, see the [virtual environments guide](https://nhsdigital.github.io/rap-community-of-practice/training_resources/python/virtual-environments/why-use-virtual-environments/).

### Running in Codespace/Google Colab

You can also load the repo into a GitHub Codespace (click the blue "Code" button and then click "Create Codespace"), or in Google Colab (see the links at the top of the page)


## Licence

This codebase is released under the MIT License. This covers both the codebase and any sample code in the documentation.

Any HTML or Markdown documentation is [© Crown copyright](https://www.nationalarchives.gov.uk/information-management/re-using-public-sector-information/uk-government-licensing-framework/crown-copyright/) and available under the terms of the [Open Government 3.0 licence](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

## Acknowledgements
- [Warren Davies](https://github.com/warren-davies4)
- [Sam Hollings](https://github.com/SamHollings)
- [Jennifer Struthers](https://github.com/jenniferstruthers1-nhs)
- Ameersohail Syed
- [The RAP team](https://github.com/NHSDigital/rap-community-of-practice)!
