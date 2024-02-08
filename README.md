# Insurance Charges Prediction Project

## Problem Statement

Insurance companies often need to estimate the charges for their customers based on various factors such as age, gender, BMI, number of children, smoking status, and region. Predicting insurance charges accurately can help insurance providers optimize pricing strategies and better manage risk.

## Project Overview

This project aims to develop a machine learning model to predict insurance charges using linear regression. The model utilizes demographic and lifestyle data to estimate insurance charges for individuals.

### Data Description

The dataset includes the following columns:

- **age**: Age of the individual (years)
- **sex**: Gender of the individual (male/female)
- **bmi**: Body Mass Index (BMI) of the individual
- **children**: Number of children/dependents covered by the insurance
- **smoker**: Smoking status of the individual (yes/no)
- **region**: Region of residence of the individual
- **charges**: Insurance charges associated with the individual

### Sample Data

| age | sex    | bmi   | children | smoker | region     | charges    |
|-----|--------|-------|----------|--------|------------|------------|
| 19  | female | 27.9  | 0        | yes    | southwest  | 16884.924  |
| 18  | male   | 33.77 | 1        | no     | southeast  | 1725.5523  |
| 28  | male   | 33    | 3        | no     | southeast  | 4449.462   |
| 33  | male   | 22.705| 0        | no     | northwest  | 21984.47061|
| 32  | male   | 28.88 | 0        | no     | northwest  | 3866.8552  |
| 31  | female | 25.74 | 0        | no     | southeast  | 3756.6216  |
| 46  | female | 33.44 | 1        | no     | southeast  | 8240.5896  |
| 37  | female | 27.74 | 3        | no     | northwest  | 7281.5056  |
| 37  | male   | 29.83 | 2        | no     | northeast  | 6406.4107  |
| 60  | female | 25.84 | 0        | no     | northwest  | 28923.13692|

## Libraries Used

- pandas
- numpy
- seaborn
- sklearn.preprocessing.LabelEncoder
- sklearn.linear_model.LinearRegression
- sklearn.metrics.r2_score
- statsmodels.stats.outliers_influence.variance_inflation_factor
- statsmodels.api
- sklearn.model_selection.train_test_split
## Step-by-Step Analysis

1. **Checking for Missing Values**: Investigated the dataset for any missing values and handled them appropriately.

2. **Assumptions of Linear Regression**: Validated key assumptions of linear regression, including linearity, normality of residuals, and homoscedasticity.

3. **Data Column Division**: Divided the dataset into numeric and categorical columns for further analysis.

4. **Checking Linearity with Scatter Plot using seaborn**: Visualized the relationship between independent and dependent variables using scatter plots.

5. **Checking Linearity with Scatter Plot using LabelEncoder**: Examined linearity after encoding categorical variables using LabelEncoder.

6. **Visualizing Outliers in "Age" Column using boxplot seaborn**: Identified and visualized outliers in the "age" column using box plots.

7. **Treating Outliers in "BMI" Column using IQR**: Detected and handled outliers in the "BMI" column using the interquartile range (IQR) method.

8. **Multicollinearity Assessment using Variance Inflation Factor (VIF)**: Checked for multicollinearity among independent variables using the VIF.

9. **Checking Correlation Among Variables**: Evaluated the correlation between independent variables and the target variable.

10. **Feature Selection Using Forward and Backward Elimination**: Employed forward and backward elimination techniques to select the most relevant features for the prediction model.

11. **Splitting the Dataset into Training and Testing Sets**: Partitioned the dataset into training and testing sets to evaluate model performance.

12. **Normalization Using Min-Max Scaler**: Normalized the training data to ensure consistent feature scaling.

13. **Prediction and Comparison of Actual vs. Predicted Charges**: Predicted insurance charges using the trained model and compared them with actual charges.

14. **Calculating R-squared Score for Predicted Charges**: Assessed the goodness-of-fit of the model by calculating the R-squared score.

15. **Checking Normality of Residuals for Linear Regression Assumption**: Verified the normality assumption of linear regression by examining the distribution of residuals.



## Conclusion

The machine learning model developed in this project demonstrates strong predictive capability in estimating insurance charges based on demographic and lifestyle factors. The model achieves a high R-squared score on the test data, indicating a good fit to the data. Overall, the project provides valuable insights into building predictive models for insurance charge estimation.


