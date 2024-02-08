# Insurance Charges Prediction Project

## Problem Statement

Insurance companies often need to estimate the charges for their customers based on various factors such as age, gender, BMI, number of children, smoking status, and region. Predicting insurance charges accurately can help insurance providers optimize pricing strategies and better manage risk.

## Project Overview

This project aims to develop a machine learning model to predict insurance charges using linear regression. The model utilizes demographic and lifestyle data to estimate insurance charges for individuals.

## Insurance Charges Dataset

This dataset contains information about individuals' demographics and healthcare charges.

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

## Step-by-Step Analysis

1. **Data Exploration**: Explored the dataset to understand its structure and characteristics, identifying features and the target variable.
   
2. **Data Preprocessing**: Performed data preprocessing tasks such as handling missing values, encoding categorical variables, and scaling numerical features.

3. **Exploratory Data Analysis (EDA)**: Analyzed relationships between variables, visualized distributions, and identified patterns in the data.

4. **Feature Selection**: Utilized techniques like correlation analysis and forward/backward elimination to select the most relevant features for the prediction model.

5. **Model Building**: Developed a linear regression model using the selected features to predict insurance charges.

6. **Model Evaluation**: Evaluated the model's performance using metrics such as R-squared, mean squared error, and mean absolute error.

7. **Assumption Checking**: Validated key assumptions of linear regression, including linearity, normality of residuals, and homoscedasticity.

## Conclusion

The machine learning model developed in this project demonstrates strong predictive capability in estimating insurance charges based on demographic and lifestyle factors. The model achieves a high R-squared score of approximately 0.741 on the test data, indicating that around 74.1% of the variance in actual insurance charges is explained by the model's predictions. Overall, the project provides valuable insights into building predictive models for insurance charge estimation.

