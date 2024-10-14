# CollegeSAT Analysis

**Author:** Rory Quinlan

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
