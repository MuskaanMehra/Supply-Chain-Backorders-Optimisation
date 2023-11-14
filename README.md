# Backorders Prediction in Supply Chain

The dataset for the project was imported from Kaggle containing 23 variables and 16 lac rows.

2 columns with large missing values (local_bo_qty and pieces_past_due) were dropped from dataset.

After cleaning data we performed EDA where we found that variables like forecast_3_month, forecast_6_month, forecast_9_month
sales_1_month,sales_3_month sales_6_month sales_9_month were highly correalted to each other so, we kept 9th month data and removed remaining variables.

Used One Hot Encoding for the categorical variables and Min Max Scaler to scale down the variables.

As our dataset had outliers and was imbalanced. Outliers were capped using IQR range and SMOTE technique was used to balance dataset.

Used Logistic regression, k-neighbors classifier, Decision tree classifier, Random forest classifier with Hyperparameter tuning to train the model.
