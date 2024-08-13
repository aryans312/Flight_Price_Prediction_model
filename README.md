**Overview-**
This project focuses on predicting airline flight prices using a machine learning approach. The goal was to apply data science and machine learning techniques to build a model with strong predictive performance.

**Dataset-**
1) Source: Kaggle's Flight Price Dataset
2) Size: 10,000+ records of flights
3) Features: Airline, Date of Journey, Source, Destination, Route, Duration, Total Stops, etc.

**Data Preprocessing-**

**Data Cleaning:**
1) Tackled null values and changed data types of time and date fields.

**Feature Engineering:**
1) Extracted hour and minute from Dep_Time, Arrival_Time, and Duration.
2) Converted Duration to minutes for uniformity.
3) Analyzed flight schedules using interactive plots (Plotly, Cufflinks)
4) Investigated the dependency of price on duration using scatter plots.
5) Analyzed airline usage on different routes.
6) Applied one-hot encoding on categorical data.
7) Performed Target Guided Encoding for airlines based on mean prices.

**Outlier Detection and Handling:**
1) Visualized outliers using boxplots and distplots.
2) Applied IQR approach to handle skewness.

**Feature Selection:** 
1) Used Mutual Information Selection to determine dependencies between variables.

**Model Selection:**
1) Trained multiple models: RandomForestRegressor, DecisionTreeRegressor.
2) Split data into 75% training and 25% testing.
3) **Made my own evaluation model** to find metrics like R², MAE, MSE, RMSE, and MAPE.

**Results:**
**1) RandomForestRegressor:**
Training Score: 0.9517
R² Score: 0.8086
MAPE: 13.27%

**2) DecisionTreeRegressor:**
Training Score: 0.9666
R² Score: 0.6813
MAPE: 15.52%

**Hyperparameter Tuning-**

**RandomizedSearchCV:**
1) Created a random grid of hyperparameters.
2) Found the best parameters, estimator, and score.

**Conclusion-**
This model provides accurate flight price predictions, with the RandomForestRegressor achieving the highest accuracy. Further tuning and more data could potentially improve performance.
