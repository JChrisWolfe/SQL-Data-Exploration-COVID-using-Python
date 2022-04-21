# COVID-19 SQL Data Exploration via Python Notebook and SQLite

## Overview
This project is used as a means to use SQL to explore COVID-19 Data. The datebase was created using the help Python to extract information from [*Coronavirus (COVID-19) Deaths*](https://ourworldindata.org/covid-deaths) by <u>**Our World in Data**</u> from <abbr title="Comma Seperated Values">CSV</abbr> files. A database was created using SQLite as the Database Management System. SQLite was chosen so that the database could be uploaded into GitHub for view for others. For easy viewing of the contents and queries of the database it was decided to use Jupyter which at the time of this writting could be viewed on GitHub without any local or remote installations of any application softwares. The results plainly put of the project only needs to be looked at from this repository.
 
There is also a related project using the data from this repository to display the information grapically using Tableau: 
1) The Github repository: `Tableau Project for COVID`
2) The Tableau site page for results from `Tableau Project for COVID`

## Required Software
While not necessary the software required the run this project are
1) Jupyter Notebook using Anaconda (it will have Python 3 included once installed)
2) SQLite

Then you would need the following Python Modules installed but would be included with the installion of Anaconda:
1) Numpy
2) Pandas
3) Sqlite3
4) Sqlalchemy

## Where to Start
The first file to look at is `initialization_COVID_DB_SQLite.ipynb`. This Python Notebook sets up the `COVID_DB.db` database needed for this project. It takes the `owid-covid-data.csv` file downloaded from <u>**Our World in Data**</u> then splits it into 2 CSV files: `CovidDeaths.csv` and `CovidVaccinations.csv`. Most of the results you'll read from `SQL Data Exploration using Python Notebook for SQLite.ipynb` is refereced from `CovidDeaths.csv` as a table.

After that take a look at `SQL Data Exploration using Python Notebook for SQLite.ipynb`. This is where SQL is used to create queries from `COVID_DB.db`. Python was used to help create SQL queries and then display the results of the queries.