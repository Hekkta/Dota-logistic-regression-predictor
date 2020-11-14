# Dota_predictor_logistic_regression
Dota is a particularly tough game to predict the outcomes for given the fast turnover of players in teams and the constant patch changes.

We explore a dataset of 5000 professional matches from datdota.com and use their elo rankings for the teams from the start date of the matches.
We can calculate the elo of each team before each match in our dataset and thus their change in elo from a week or month prior the game, we'll use this  to measure the teams form.

Once the data is collected, tidied and sorted we train a logistic regression model on 80% of the dataset and test on the remaining 20% by attempting to predict the outcome of each game from the elo and form of each team.
We use the Jaccard index and log loss scores as measurements of our success.
