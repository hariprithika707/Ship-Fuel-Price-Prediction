**Ship Fuel Consumption Prediction**
**Overview**
This project focuses on predicting ship fuel consumption based on the mean draft of the ship. The model is built using Lasso regression, providing an accurate prediction system that can be used to improve fuel efficiency.
Model Details
Input
Mean Draft: The vertical distance between the waterline and the bottom of the ship’s hull, which indicates the draft of the ship.
Output
Fuel Consumption: The predicted fuel consumption based on the provided mean draft value.
Model
Lasso Regression: A linear regression model with L1 regularization (Lasso) to minimize the overfitting of irrelevant features.
Dataset
The model was trained on a dataset containing records of ships' drafts and corresponding fuel consumption data. This dataset is not included in the repository for privacy reasons.

Results
The Lasso model is able to predict the ship's fuel consumption with a good degree of accuracy, based solely on the mean draft. Additional features such as weather conditions or cargo weight can be included in future work for improved accuracy.
