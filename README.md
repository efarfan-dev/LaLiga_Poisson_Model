# LaLiga_Poisson_Model
# La Liga Match Predictor (v1)

This project uses a Poisson distribution to forecast soccer match outcomes. It is built to explore how statistical modeling can be applied to real world sports data.

## Data Source
Historical match results are pulled from [Football-Data.co.uk](https://www.football-data.co.uk/), specifically focusing on the Spanish La Liga.

## How it works
The model uses a Generalized Linear Model (GLM) to analyze match history and predict future results. Instead of just picking a winner, it calculates:
Team Strength:Individual attack and defense ratings for each team based on past performance.
Home Advantage:The specific statistical boost a team gets when playing at home.

The model generates a probability matrix for every possible scoreline (ex. 2-1, 1-1, 0-3). By summing the values in this matrix, we can determine the exact percentage chance for a home win, a draw, or an away win.

## Tech Used
Google Colab: Primary development environment.
Python: (Pandas, NumPy, Statsmodels, Scipy).
Seaborn: Used to generate probability heatmaps for score predictions.

## Use the Model
Since this was built in Google Colab, you can open the notebook directly and run it in your browser. You can swap team names in the code to generate predictions for any matchup in the dataset.

## Future Plans
This is Version 1. I am currently learning how to improve the accuracy of these predictions and plan to build an updated version for the 2026 World Cup that accounts for current form and player availability. I will also try to test it for every match from now till the end of the LaLiga season and post the accuracy.
