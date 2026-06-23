Traffic Volume Prediction Using Ensemble Learning Techniques

This project aims to predict traffic volume using ensemble learning algorithms. Three ensemble models—Random Forest, AdaBoost, and XGBoost—were implemented and compared using the Metro Interstate Traffic Volume dataset. The objective was to determine which ensemble method provides the most accurate traffic volume predictions.

Dataset Used:
The Metro Interstate Traffic Volume dataset was obtained from the UCI Machine Learning Repository. The dataset contains hourly traffic volume records collected from Interstate 94 in Minneapolis, Minnesota, along with weather and holiday-related information.

#Original Features

| Feature             | Description                      |
| ------------------- | -------------------------------- |
| holiday             | Holiday information              |
| temp                | Temperature (Kelvin)             |
| rain_1h             | Rainfall in the last hour        |
| snow_1h             | Snowfall in the last hour        |
| clouds_all          | Cloud coverage percentage        |
| weather_main        | Main weather category            |
| weather_description | Detailed weather description     |
| date_time           | Date and time of observation     |
| traffic_volume      | Traffic volume (target variable) |

Data Preprocessing and Missing Value Handling

Data preprocessing was performed to improve model performance and prepare the dataset for machine learning algorithms. The holiday column contained a large number of missing values because most days were not holidays. Missing values were replaced with the category "None".

After feature extraction, the original date_time column was removed.

Encoding Variables
The categorical columns holiday, weather_main, and weather_description were transformed into numerical values using Label Encoding.

#Train and Test data
The dataset was divided into:

* Training set: 80%
* Testing set: 20%

A random state of 42 was used to ensure reproducibility.

RANDOM FOREST
Random Forest is a bagging-based ensemble algorithm that constructs multiple decision trees and combines their predictions through averaging. It reduces overfitting and improves generalization performance.

ADABOOST
AdaBoost (Adaptive Boosting) is a boosting algorithm that trains weak learners sequentially. Each new model focuses on correcting errors made by previous models.

XGBOOST
Extreme Gradient Boosting (XGBoost) is an advanced boosting algorithm that uses gradient descent optimization, regularization techniques, and efficient tree construction to improve predictive performance.

Results
The performance of each model was evaluated using:
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* Coefficient of Determination (R²)

| Model         |    MAE |   RMSE | R² Score |
| ------------- | -----: | -----: | -------: |
| Random Forest | 198.05 | 364.40 |   0.9664 |
| AdaBoost      | 629.40 | 836.09 |   0.8232 |
| XGBoost       | 223.49 | 374.95 |   0.9644 |


This project successfully implemented and compared three ensemble learning techniques for traffic volume prediction using the Metro Interstate Traffic Volume dataset. Data preprocessing, feature engineering, and model evaluation were conducted to assess model performance.

Among the three algorithms, Random Forest achieved the best results with an R² score of 0.9664, followed closely by XGBoost with an R² score of 0.9644. AdaBoost demonstrated comparatively lower performance.

The findings indicate that ensemble learning techniques, particularly Random Forest and XGBoost, are highly suitable for traffic volume forecasting applications and can support intelligent transportation systems in making data-driven decisions.
