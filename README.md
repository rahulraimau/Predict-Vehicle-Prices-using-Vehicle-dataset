Vehicle Price Prediction Project Report/Readme
Project Goal
The goal of this project is to build a machine learning model to predict vehicle prices based on various features.

Steps Performed
Imports: Imported necessary libraries for data manipulation, visualization, and machine learning.
Load Dataset: Loaded the vehicle dataset from a CSV file.
Drop Unused Text Columns: Removed text-based columns that were not used in the model.
Drop rows where target 'price' is missing: Handled missing target values by removing the corresponding rows.
Fill Missing Values: Imputed missing values in numerical and categorical columns using median and mode respectively.
One-Hot Encoding: Converted categorical features into numerical format using one-hot encoding.
Feature/Target Split: Separated the dataset into features (X) and target (y - price).
Train-Test Split: Split the data into training and testing sets for model development and evaluation.
Model Training (Random Forest): Trained a Random Forest Regressor model on the training data.
Random Forest Evaluation: Evaluated the Random Forest model using R^2 and RMSE metrics.
Model Training (XGBoost): Trained an XGBoost Regressor model, including cleaning feature names for compatibility.
XGBoost Evaluation: Evaluated the XGBoost model using R^2 and RMSE metrics.
Feature Importance from Random Forest: Visualized the top 10 most important features from the Random Forest model.
SHAP Explainability for XGBoost: Generated a SHAP summary plot to explain the XGBoost model's predictions.
Save Models: Saved the trained Random Forest and XGBoost models to pickle files.
Results
The Random Forest model achieved an R^2 score of 0.7985 and an RMSE of 7844.55 on the test set.

The XGBoost model achieved an R^2 score of 0.8187 and an RMSE of 7440.43 on the test set.

Based on these metrics, the XGBoost model performed slightly better in predicting vehicle prices.

Visualizations
Top 10 Feature Importances (Random Forest): A bar plot showing the relative importance of the top 10 features as determined by the Random Forest model.
SHAP Summary Plot (XGBoost): A plot illustrating the impact of features on the XGBoost model's output, providing insights into how each feature affects the price prediction.
Saved Models
The trained models are saved as vehicle_price_predictor_rf.pkl and vehicle_price_predictor_xgb.pkl. These can be loaded and used for making predictions on new data.
