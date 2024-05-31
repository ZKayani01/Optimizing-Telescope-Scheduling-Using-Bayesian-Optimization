Optimizing Telescope Scheduling Using Bayesian Optimization


The goal of this project is to optimize telescope scheduling to maximize the scientific value of astronomical observations. This involves developing a machine learning model to predict the optimal schedule based on various factors such as weather conditions, celestial object visibility, and scientific priority. The model will leverage Bayesian optimization for hyperparameter tuning to ensure the best performance.

I am using the SDSS data set to observe historical logs, NOAA to observe weather data and Gaia mission for astronomical object catalogues. 

For optimizing telescope scheduling, we chose the Random Forest Regressor. This model is suitable due to its robustness in handling complex datasets and its ability to model non-linear relationships effectively. Random Forest is an ensemble learning method that constructs multiple decision trees and merges them to get a more accurate and stable prediction. 

## HYPERPARAMETER OPTIMSATION
The hyperparameters I ised are:
Number of Estimators, Max Depth, Minimum Samples Split, Minimum Samples Leaf, Max Features

We used Bayesian Optimization to find the optimal hyperparameters. Bayesian Optimization is suitable for hyperparameter tuning because it builds a probabilistic model of the objective function and uses it to select the most promising hyperparameters, balancing exploration and exploitation.

## RESULTS
The model's performance was evaluated using Mean Squared Error (MSE) on the validation and test sets. 

The results indicate that the model generalizes well to unseen data, suggesting that it can effectively predict optimal telescope scheduling. The feature importance analysis revealed that weather conditions and certain celestial object characteristics were the most significant predictors, which aligns with domain knowledge in astronomy.


