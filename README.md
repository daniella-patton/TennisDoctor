# TennisDoctor
An injury predictor for female professional tennis players. 

Last Edit: 1/31/20
Boston Health Data Science Insight Fellow Project Jan - April 2020

# Motivation
Female professional tennis players face a grueling and time consuming schedule. Their are over 36-weeks of WTA tournaments scheduled for 2020 alone. Further, their is only ~6 weeks of off-season in a given year. Given the gureling tennis season, injuries are both common and frequent amongst the top 200 players. This project predicts the risk of future injury (i.e., in the next three months) of tennis players based off of previous match and injury, and raaking history.  

This reposiitory contains all of the base code for this project. 

# Data Collection
Code: Extracting_Files-Sqlite.ipynb

This file creates a database in sqlite by pulling out information for female professional tennis players from 2010 - 2020. More specifically, this database largely relies on data from www.tennisexplorer.com to extract match, injury, and rank history. In addition, basic demographic data was recorded for each player when present. Data was pulled specifically from the top 200 players from 2010 - 2020. Court type data was extracted from a database created by JeffSackmann (tennis_wta) off of github.

__The following tables will be created in this database:__
* __Players__ (name, birthday, current/highest singles and doubles ranking, hand, sex, height, and weight)
* __Injury_Record__ (name_id,start_date,end_date, tournament,reason )
* __Match_Record__ (name_id, year, tournament, match_type, date, opponent, round, result, h ,a)
* __Ranks__ (name_id, year, ranktype, rank
* __Court_Type__ (Tournament, Court Type)

# Credits
Data used for this project was pulled from two seperate sources: www.tenisexplorer.com and from JeffSackmann (tennis_wta) off of github.

# License
MIT @ Daniella-Patton
