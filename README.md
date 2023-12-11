# Boom Bike Sharing Multiple Linear Regression Model
> This repository contains code and resources to build a multiple linear regression model for predicting bike rental counts in a bike-sharing system.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Model Building](#model-building)
* [Conclusions](#conclusions)


## General Information
The dataset used for this analysis contains information on various factors that might influence bike rental demand. It includes features like season, weather conditions, temperature, humidity, and more. The 'cnt' column represents the total number of bike rentals for a given day, including both casual and registered users.


## Technologies Used
- Python 3.11.5
- Pandas 2.0.3
- Numpy 1.24.3
- Matplotlib 3.7.2
- Seaborn 0.12.2
- Statsmodels 0.14.0
- Scikit-learn 1.3.0


## Model Building
Data Preparation:
Categorical variables like 'season' and 'weathersit' were converted into string values to better represent their categories.
The dataset was split into training and testing sets.
Model Training:
Utilized the multiple linear regression technique using Python and the Statsmodels library.
Conducted feature selection, assessing the significance of variables for predicting bike rental counts.

Model Evaluation
Performance Metrics:
Evaluated the model using R-squared score on the test set.
Observed an R-squared score of around 0.806, indicating the model explains about 80.6% of the variance in bike rental counts.

Significant Variables:
Identified significant variables such as 'season', 'yr', 'weathersit', 'atemp', 'hum', 'windspeed', etc., impacting bike rentals.



## Conclusions
Model Fit: The model shows a relatively good fit as indicated by the R-squared value of 0.806, implying that approximately 80.6% of the variability in the dependent variable ("cnt" - bike rentals) is explained by the independent variables included in the model.

Significant Predictors: Several predictors such as "season," "yr" (year), "mnth" (month), "weekday," "weathersit," "atemp" (feels-like temperature), "hum" (humidity), "windspeed," "day," "month," and "year" exhibit significant relationships with the number of bike rentals ("cnt").

Intercept and Coefficients: The intercept (constant) has a coefficient of -42.4755, implying the expected value of "cnt" when all predictors are zero. Each coefficient represents the change in the dependent variable for a unit change in the respective predictor, holding other predictors constant.

P-values: Most predictors have p-values less than 0.05, indicating their statistical significance in predicting bike rentals. However, the predictor "day_of_week" has a p-value of 0.807, suggesting it might not significantly contribute to the model.

Multicollinearity: The note about the smallest eigenvalue being close to zero or singular design matrix suggests potential multicollinearity issues among predictors. Strong multicollinearity might affect the stability and interpretability of the coefficients.


## Contact
Created by [@kpavan3697] - feel free to contact me!
