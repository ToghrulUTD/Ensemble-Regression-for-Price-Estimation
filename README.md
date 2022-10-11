# Ensemble-Regression-for-Price-Estimation

## Dataset
The dataset was assembled in January 2022. Data from a well-known car sale site in Poland (which is public). Selenium and request were used for parsing.

The dataset contains information about the make, model, generation, year of production, mileage, engine type and volume, localization and price

## Methods Used

In this project, I have cleaned the dataset by filling missing values, removing $ signs and other characters from numerical variables, carried out feature engineering, and transformed the skewed data using log and sqrt transformations to reduce the impact of outliers for price prediction. I have also encoded categorical features with dummy and target encoding techniques. Next, I have implemented linear methods such as GLM, Ridge and Lasso regressions. For the final model, I have chosen Gradient Boosting regressor with LightGBM module as linear models perform poor due to the categorical features. I have implemented tuning for the final model, and explained the regression errors using SHAP contributions, and build surrogate tree for residual analysis. Lastly, I have created a performs function that combines all the above steps, training and predicting unseen data. The steps are the following:

1. **Load, Clean, Preprocess, and Feature Engineer**
2. **Linear Regression**
3. **Gradient Boosting regression and tuning**
4. **Model explainability**
5. **Residual Analysis**
6. **Final Pipeline**
