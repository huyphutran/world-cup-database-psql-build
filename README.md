# 💻 Project: WorldCup Database 

# World Cup Database

## Overview
This database contains information about participating teams and matches in the FIFA World Cup tournament.

## Data Structure
The database consists of two main tables:

1. **Teams**: Information about participating teams such as team name, country, coach, etc.
2. **Games**: Details about each match including match date, location, teams playing, scores, etc.

## Database Schema
The database schema is as follows:

- **Teams**
  - team_id (Primary Key)
  - team_name

- **Games**
  - game_id (Primary Key)
  - year
  - home_team_id (Foreign Key referencing Teams)
  - away_team_id (Foreign Key referencing Teams)
  - home_team_score
  - away_team_score

 ## Automating data insertion and querying with SQL
Created a Bash script that reads the games.csv data and uses SQL query commands to insert the data automatically into the tables previously created.

Took constraints into consideration when creating the Bash script to insert all winner and opponent teams individually into 'teams' and then into 'games' based on the team_id created.

View: <a href="https://github.com/huyphutran/world-cup-database-psql-build/blob/main/insert_data.sh"> insert_data.sh
  </a>
Finished by writing a Bash script that utilises SQL to query the database and obtain useful values.

View: <a href="https://github.com/huyphutran/world-cup-database-psql-build/blob/main/queries.sh"> queries.sh
  </a>
