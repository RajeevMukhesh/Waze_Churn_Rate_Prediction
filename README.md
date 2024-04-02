# Waze's Churn Rate Prediction

# Overview
This project objective is to determine the user churn rate of the Waze app. This project unitlized a synthetic data created in partnership with Waze. The dataset is trained on Random Forest Classifier and XGBoost Classifier models. The results were poor for both the models with XGBoost performing slightly better with a recall score of 0.14 on the original dataset. The rebalanced (upsampled) dataset resulted on ~85% jump in the recall score of 0.97. The XGBoost model used most of the engineered features in its prediction with km_per_hour (kilometers driven per hour) being the most predictive feature.

# Business Understanding
Waze’s free navigation app makes it easier for drivers around the world to get to where they want to go. Waze’s community of map editors, beta testers, translators, partners, and users helps make each drive better and safer. Typically, high retention rates indicate satisfied users who repeatedly use the Waze app over time. Developing a churn prediction model will help prevent churn, improve user retention, and grow Waze’s business. An accurate model can help identify specific factors that contribute to who, why and when users churn so that Waze can proactively engage these users with special offers to retain them.

# Data Understanding
The dataset contains ~15K records with 12 features. The features include information on the user drives, sessions, activity, favorite navigations and duration of drives.

# Modelling and Evaluation
While the logistic regression indicated activity days as the most predictive feature, random forest and xgboost models utilized most the engineered features in their predictions. The xgboost model slightly outperformed the random forest model with a recall score of 0.969 and F1 score of 0.914 (on the upsampled dataset). The model is not overfit as it produced similar results on the both validation and test datasets.

# Conclusion
The model predicted churn rate of the data based on kilometers driven per hour and per day. The original data scores were low and greatly improved upon upsampling the data which indicates that more data from the Waze would result in improved model performance. Also, more engineered features in collaboration with the domain experts would result in model's performance as most the features included in prediction were feature engineered.
