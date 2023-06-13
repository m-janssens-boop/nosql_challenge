# nosql_challenge

This repository contains two jupyter notebooks, NoSQL_setup.ipynb and NoSQL_analysis.ipynb.

NoSQL_setup.ipynb uses MongoDB to import a JSON file of data on various establishments conatined in different geographical locations and create a database. It then uses PyMongo to update, parse, and clean the data within the database. NoSQL_analysis.ipynb uses the updated database, PyMongo, and Pandas to perform exploratory analysis on the establishments collection in the database. Different dataframes are compiled using various criteria (including hygiene scores, proximity to other establishments, and rating values).