# CollegeSAT Analysis

## Table of Contents

1. [Overview](#overview) 
2. [Plots and Model Fitting](#plots-and-model-fitting)
   - [Raw Data Analysis](#1-raw-data-analysis)
   - [Transformed Data Analysis](#2-transformed-data-analysis)
3. [Conclusion](#conclusion)
   - [Violations of Linear Regression Assumptions in the Original Data](#violations-of-linear-regression-assumptions-in-the-original-data)
   - [How the Transformation Addresses These Violations](#how-the-transformation-addresses-these-violations)

## Overview

This project analyzes college acceptance rates in relation to SAT scores. It involves creating visualizations, fitting models on both raw and transformed data, and evaluating residuals.

## Plots and Model Fitting

### 1. Raw Data Analysis

- **Histogram of Acceptance Rates**: A histogram visualizes the distribution of acceptance rates with customized colors and labels.
  
- **Scatterplot of SAT vs. Acceptance Rate**: A scatterplot illustrates the relationship between SAT scores and acceptance rates.

- **Linear Model**: A linear regression model is fitted to predict acceptance rates based on SAT scores. Predictions and residuals are calculated.

- **Residual Plot**: A plot of predicted acceptance rates against jackknife residuals helps evaluate the model's performance.

- **Normal Q-Q Plot**: This plot assesses the normality of residuals.

### 2. Transformed Data Analysis

- **Logit Transformation**: The acceptance rate is transformed using the logit function to better meet model assumptions.

- **Histogram of Transformed Acceptance Rates**: A histogram shows the distribution of transformed acceptance rates.

- **Scatterplot of SAT vs. Transformed Acceptance Rate**: This scatterplot illustrates the relationship after transformation.

- **Transformed Linear Model**: A

- **Normal QQ Plot**:

<br>

<div style="display: flex;">
    <img src="https://github.com/RoryQo/College-Acceptance-and-SAT-Scores/raw/main/PreQQ.jpg" style="width: 400px; margin-right: 10px;" alt="Pre Transformation Q-Q Plot">
    <img src="https://github.com/RoryQo/College-Acceptance-and-SAT-Scores/raw/main/QQ.jpg" style="width: 400px;" alt="Post Transformation Q-Q Plot">
</div>

<br>
<br>

The analysis highlights the importance of considering the underlying assumptions of linear regression when modeling acceptance rates as a function of SAT scores. 

## Conclusion

### Violations of Linear Regression Assumptions in the Original Data

- **Linearity**: The initial scatterplot suggested a linear relationship, but the residuals plot indicated that the residuals were not evenly distributed around zero, pointing to potential non-linearity in the data.

- **Homoscedasticity**: The residual plot for the raw model displayed a pattern indicating heteroscedasticity, where the variance of residuals increased with the fitted values. This violates the assumption that the residuals should have constant variance.

- **Normality of Residuals**: The Q-Q plots for the raw residuals showed noticeable deviations from the diagonal line, suggesting that the residuals were not normally distributed, which is a key assumption of linear regression.

### How the Transformation Addresses These Violations

The logit transformation applied to the acceptance rates helps to rectify these violations:

- **Linearity**: By transforming the acceptance rates, the relationship between SAT scores and the transformed acceptance rates becomes more linear, improving the fit of the model.

- **Homoscedasticity**: The transformation stabilizes the variance of residuals, leading to a more consistent spread across the range of fitted values, thus addressing the issue of heteroscedasticity.

- **Normality of Residuals**: The logit transformation improves the distribution of the residuals, bringing them closer to a normal distribution, which is crucial for the validity of hypothesis tests and confidence intervals in regression analysis.

Overall, while the original model provided insights into the relationship between SAT scores and acceptance rates, the transformation significantly improved the model's adherence to linear regression assumptions, resulting in a more reliable and interpretable analysis.
