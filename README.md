# Predicting NFL Game Results with Elo Ratings

## Project Summary
FiveThirtyEight has created Elo ratings as a way to measure the strengths of home and away teams based on previous games. We are interested in using these Elo ratings in predicting the results of a game. Through our analysis, we used logistic regression to predict the odds of the home team winning using the differences in Elo ratings between home and away teams, to see if the home team has a significant advantage.

## Data Dictionary
Here are the variables that we will be using for our analysis:

| Variable  | Description               |
|:----------|:--------------------------|
| elo1_pre | Home team's Elo rating before the game |
| elo2_pre | Away team's Elo rating before the game |
| elo_diff | Home team's Elo rating before the game minus the Away team's Elo rating before the game (elo1_pre - elo2_pre) |
| qb1_value_pre | Home starting quarterback's raw Elo value before the game |
| qb2_value_pre | Away starting quarterback's raw Elo value before the game |
| qb1_value_post | Home team starting quarterback's raw Elo value after the game |
| qb2_value_post | Away team starting quarterback's raw Elo value after the game |
| qb_diff_pre | Home team starting quarterback's raw Elo value before the game minus Away team starting quarterback's raw Elo value before the game (qb1_value_pre - qb2_value_pre) |
| qb_game_diff | Change in Home team starting quarterbacks' raw Elo less change in Away team starting quarterbacks' raw Elo. A measurement of by how much one quarterback outperformed the other in a given game (qb1_value_post - qb1_value_pre) - (qb2_value_post - qb2_value_pre). |
| score1 | Home team's score |
| score2 | Away team's score |
| score_diff | The difference between score1 and score2 (score1-score2) |
| playoff | Whether game was in playoffs, and the playoff round if so |
| playoff_bin | Whether or not the game was a playoff game (1: yes, 0: no) |
| result | Whether or not the home team won (1: yes, 0: no) |
