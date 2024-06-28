# Park & Ride Analysis Darmstadt

The following repositories does a data analysis to asses the current park & ride demands in Darmtadt.

## Installation: 


Following dependencies are required for the project: 

* Python ^3.12 ([PyEnv](https://github.com/pyenv/pyenv) can be used)
* [Poetry](https://python-poetry.org/) ^1.8

Use Poetry to create a virtual environment and install all dependencies with:

```bash
poetry install
```

Note: For IDE support, it needs to find the virtual environment created by poetry. This works better, most of the time automatically, if you [configure poetry](https://python-poetry.org/docs/configuration/#virtualenvsin-project) to create the virtual environment within the project prior to running above command.

The virtual environment needs to be activated. One possibility is to spawn a new shell with: 

```bash
poetry shell
```

In the rest of the README it is assumed that all commands are executed within this shell.

## Data Preparation

To process the raw commuters data `19321-Z-22` from the ("Statistische Ämter des Bundes und des Landes")[https://www.regionalstatistik.de] execute the notebook `park_and_ride_analysis.notebooks.preprocess_data.ipynb`.

To download some road data for Darmstadt and its sourroundings execute the `park_and_ride_analysis.notebooks.map_data.ipynb` notebook.

## Data Analysis

To run the data analysis run the `park_and_ride_analysis.notebooks.analyse_data.ipynb` notebook.