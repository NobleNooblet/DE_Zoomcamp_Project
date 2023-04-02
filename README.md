![](images/esports_logo.jpg)

## Project Description / Problem Description
Ask any young child what they want to do when they grow up and you'll find that, in some cases, the answer will be to play video games or to become a content creator.  In today's day and age it's not uncommon for young (or even older) individuals to pursue a career in the video game industry.  Playing video games professionally is one way to make a living, but unfortunately, just like any other sport/activity, you'll need to be one of the best players in the world to make it to the professional gaming scene called Esports. Esports , short for electronic sports, is a form of competition using video games.  Esports often takes the form of organized, multiplayer video game competititons, particularly between professional players, individually or as a team.

![](images/esports_sub_logo.jpg)

The aim of this project is to give the user insight on the possibilities of: 1. The financial gain by playing video games in a professional manner and 2.  To indicate to the user, which might still be deciding on a game to participate in, which games on the e-sports scene is the most rewarding by looking at the top earnings per game and game genre and 3.  Provide the user with a geographical distribution of the top earners for these specific games/genres in order provide insights on which regions are more likely to support specific games in the competitive scene.  

The project will gather, process and display esport earnings data of the top 100 earners for ten specific games found in the esport scenery.  More information on the data gathering, processing and displaying steps are discussed further in this document.

## Data set
The data that will be used for this project can be found on kaggle.com - [Link](https://www.kaggle.com/datasets/jackdaoud/esports-earnings-for-players-teams-by-game).  The main two files we are interested in are the following:
* highest_earning_players.csv
    * Provide the player's detail, game the player plays.
* country-and-continent-codes-list.csv
    * Provide the geographical information that can be linked to the player's country code

The final dashboard can be viewed by opening this [LINK](https://lookerstudio.google.com/s/sBzaz4soa7I)

## High level project design
The puprose of this section is to illustrate the data pipeline architecture of this project via the following image:

![](images/overall_design.jpg)




## Technologies used:
* Code: Python
* Terraform
    * Infrastructure code that provisions:
        * Google Cloud Storage Buckets
        * Google Big Query Data Sets
* Google Cloud Platform
    * Google Cloud Storage (storing raw data files)
    * Google Big Query (Data Warehouse)
* Prefect
    * Orchestrator tool for the data pipeline
* DBT
    * Data transformation and deployment into the production warehouse data set
* Data Visualization
    * Looker Studio