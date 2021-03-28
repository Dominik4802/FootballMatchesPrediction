# Predicting the outcome of the football matches

## Description of the problem 

We would like to create a model which predicts the results of the football matches from perspective of a home team (win, defeat, draw) in one of the most famous football leagues in the world - La Liga (Football league in Spain). Our predictions will be based on statistics from previous matches and seasons, bets created by the worldwide betting sites and other available statistics. <br>
In the report we would like to present few methods of handling this problem and compare them based on different performance measures. <br>
This model will bring some valuable insight for sports experts and coaches before important matches as well as people willing to bet on a match result.
<br>
<br>
## Some of the approaches solving the problem (found in literature):
- [Predicting results based on Twitter information](https://arxiv.org/pdf/1411.1243.pdf)
- [Post predicts football matches using the Poisson distribution](https://dashee87.github.io/football/python/predicting-football-results-with-statistical-modelling/)
- [Predicting results based on web search engine](https://qz.com/233830/world-cup-germany-argentina-predictions-microsoft/)
- [Different Machine Learning techniques used to predict results](https://www.imperial.ac.uk/media/imperial-college/faculty-of-engineering/computing/public/1718-ug-projects/Corentin-Herbinet-Using-Machine-Learning-techniques-to-predict-the-outcome-of-profressional-football-matches.pdf)
- [Predicting results based on player ratings from EA Sports](https://towardsdatascience.com/predicting-premier-league-odds-from-ea-player-bfdb52597392)
<br>

## Our approach
We would like to meet the problem of predicting results based on general statistics of historical matches, as well as, statistics of every team provided in FIFA 11, FIFA 15, FIFA 16 available in the following data source: <br>
https://www.kaggle.com/hugomathien/soccer

### Input parameters:
- attributes of home team and away team provided by FIFA (of release date the closest to the match day):
    - dribbling,
    - speed,
    - passing
    - positioning, 
    - crossing, 
    - shooting, 
    - pressure, 
    - aggression;
- bets made on the match result by betting sites (we took the average from all available sites)
- points scored in the last matches with this exact opponent
- results of recently played matches of home team and away team

### Output:
The predicted outcome of the match (win of the home team, defeat of the home team, or a draw).
<br>
<br>

### Methods used:
1.	Logistic regression
2.	XGBoost
3.	Random Forest

### Indexes used to assess the methods:
- Accuracy (number of correct predictions over total number of predictions)
- F1 Score

<br>

# Authors:

Dominik Jakubowski <br>
Michał Laskowski <br>