# Disaster Response Pipeline Project

## This Project is part of Data Science Nanodegree Program by Udacity in collaboration with Figure Eight. The dataset contains pre-labelled tweet and messages from real-life disaster events. The project aim is to build a Natural Language Processing (NLP) model to categorize messages on a real time basis.

## This project is divided in the following key sections:

## Processing data, building an ETL pipeline to extract data from source, clean the data and save them in a SQLite DB
## Build a machine learning pipeline to train the which can classify text message in various categories
## Run a web app which can show model results in real time

### Instructions:
### Data
## process_data.py: reads in the data, cleans and stores it in a SQL database. Basic usage is python process_data.py 
## categories.csv and messages.csv (dataset)
## YourDatabaseName.db: created database from transformed and cleaned data.

### Models
## train_classifier.py: includes the code necessary to load data, transform it using natural language processing, run a machine learning model using GridSearchCV and train it.      ## Basic usage is python train_classifier.py DATABASE_DIRECTORY SAVENAME_FOR_MODEL
### App
## run.py: Flask app and the user interface used to predict results and display them.
## templates: folder containing the html templates

### How to run:

python process_data.py messages.csv categories.csv YourDatabaseName.db

python train_classifier.py ../data/YourDatabaseName.db classifier.pkl

python run.py
