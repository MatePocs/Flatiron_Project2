# Flatiron Module 2 Project¶
Work of Mate Pocs, January 2020.

Introcution
Purpose of the project is to explore the Football Delphi database from kaggle (https://www.kaggle.com/laudanum/footballdelphi), run SQL queries on it, obtain weather information from Dark Sky API, and at the end of the project, create a MongoDB database in the following structure:

The name of the team
The total number of goals scored by the team during the 2011 season
The total number of wins the team earned during the 2011 season
A histogram visualization of the team's wins and losses for the 2011 season (store the visualization directly by assigning it to a variable)
The team's win percentage on days where it was raining during games in the 2011 season.

The project has the following structure:

Section 1 - SQL Infrastructure: Importing libraries and setting up a class that will handle the SQL queries.

Section 2 - Data Exploration: Exploring the databases, by running SQL queries. By the end, we will have a Pandas DataFrame containing information of the relevant matches, and another DataFrame we will use to document the daily weather conditions.

Section 3 - API Structure Exploration: In this section, we are setting up the API key, and exploring the possibilities of the Dark Sky API. We look into the json data and try to come up with a good algorithm that signals if it was raining on a particular day.

Section 4 - Saving Weather Information: This is the section where we request weather information for the dates when matches were played in the 2011 season. First, we get the json data information, and save that for future reference. Then, we run a method that decides if it was raining on a particular day. We are saving the rainy day indicator file in a csv.

Section 5 - Combining the Data: We create a combined dataframe of the two main dataframes we got as a result of the previous sections. The combined database will contain the names of the different teams in one column, and the requested statistics in the other columns.

Section 6 - MongoDB: We create a new MongoDB database and enter the combined results.

Files in the repository:

index.ipynb: Jupyter Notebook, detailed documentation of the project 

database.sqlite: original database from Kaggle

season_2011_rainy_days.csv: a table documenting whether the weather was rainy or not on a certain day
