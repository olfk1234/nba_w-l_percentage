In this project, I aim to use the a regression machine learning model to determine the W/L percentage of NBA teams at the end of the season based on team ranking stats found on https://www.basketball-reference.com/.
Data from the 2002-2003 season until the 2021-2022 season was used. Predictions were made for the 2022-2023 season for the winning percentage and record for all teams.
The following steps were done:
1) The main data was imported and feature engineering was done to ensure that the data could be utilized by the algorithm.
2) A 90%/10% train test split was done to ensure that test data would be available to evaluate performance
3) The data was scaled so that differences in the units of the column would not affect the machine learning algorithm.
4) A grid search cross validataion method was done on a variety of machine learning algorithms to determine the optimal hyperparamters that would yield the lowest error.
  - The machine learning model with the lowest mean square root error and lowest mean absolute error was used for the mid-season data from the 2022-2023 season. 
5) The optimal model and the scaler were dumped into separate joblib files, which can be accessed in a separate file to use the machine learning model.

https://www.basketball-reference.com/leagues/NBA_2022_ratings.html - This URL is the dataset for the 2022-2023 season. Hovering over each of the headers in the table on this page will explain all the statistics used in the machine learning algorithm.
