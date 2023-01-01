In this project, I aim to use the KNearestNeighbor Regressor to determine the W/L percentage of NBA teams at the end of the season based on stats found on https://www.basketball-reference.com/.
Data from the 2002-2003 season until the 2021-2022 season was used. Predictions were made for the 2022-2023 season for the winning percentage and record for all teams.
The following steps were done:
1) The main data was imported and feature engineering was done to ensure that the data could be utilized by the algorithm.
2) A 70%/30% train test split was done to ensure that test data would be available to evaluate performance
3) The data was scaled so that differences in the units of the column would not affect the machine learning algorithm.
4) A grid search cross validataion method was done on a KNearestNeighborsRegressor model to determine the optimal nearest neighbors hyperparamter that would yield the lowest error.
  - The KNearestNeighborsRegressor was used because this model provides a low mean square root error and mean absolute error with a low computing time.
5) An instance of the model was made with the optimal nearest neighbor value. 
6) The model and a scaler was dumped into separate joblib files, which can be accessed to use the machine learning model.
