# car-price-prediction

The provided code outlines the steps for car price prediction using machine learning with the following major steps:

# 1. Data Preparation:
   - Loading the dataset and cleaning it by removing irrelevant columns and handling missing and duplicate values.
   - Encoding categorical variables using `LabelEncoder` to convert text data into numeric values.
   - Feature engineering, where a new binary column is created (`Turbo`), and the 'Engine volume' is cleaned and converted to `float`.

# 2. Model Training:
   - Split the dataset into training and test sets using `train_test_split`.
   - Trained three models:
     - Linear Regression
     - Random Forest Regression
     - Gradient Boosting Regression
   - Evaluation of models using metrics like `Mean Squared Error (MSE)` and `R-squared`.

# 3. Model Evaluation:
   - Visualized the performance of the models by plotting actual vs. predicted prices.
   - Compared `MSE` values and calculated variance of the target variable (`Price`) to evaluate model performance.

# 4. Model Saving:
   - Saved the trained Random Forest model (`rf_model`) using `pickle` for future use.
   - Added placeholders for saving other preprocessing components like the `LabelEncoder`.

# Key Improvements & Additions:
- Feature Scaling: It would help to scale features (especially when using algorithms like Linear Regression) to improve performance.
- Hyperparameter Tuning: For Random Forest and Gradient Boosting, tuning parameters can improve accuracy.
