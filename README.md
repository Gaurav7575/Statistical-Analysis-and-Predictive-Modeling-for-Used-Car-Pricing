# Statistical-Analysis-and-Predictive-Modeling-for-Used-Car-Pricing
Analyzing factors influencing Toyota Hilux prices (2018-2022) using AutoTrader UK data with visualization, regression, hypothesis testing, and predictive modeling to uncover pricing trends and predict prices.

# Statistical Analysis and Predictive Modeling for Used Car Pricing

## Overview

This project focuses on analyzing the factors influencing the price of second-hand Toyota Hilux vehicles using data sourced from [AutoTrader UK](https://www.autotrader.co.uk). The study spans vehicles registered between 2018 and 2022, avoiding outliers from newer models. By leveraging statistical and predictive modeling techniques, the project identifies key factors impacting pricing and predicts vehicle prices based on features like mileage, engine power, and registration year.

## Features

- **Data Visualization**:
  - Distribution of car registrations and their mileage.
  - Scatterplots and boxplots highlighting correlations between price, mileage, and registration year.
- **Statistical Analysis**:
  - Hypothesis testing to validate pricing trends.
  - Confidence interval estimation for price predictions.
  - Correlation and regression analysis to uncover significant relationships.
- **Predictive Modeling**:
  - Linear regression model with an R² value of 0.851.
  - Prediction of car prices using key independent variables.
- **Residual Analysis**:
  - Validation of model assumptions, including linearity, homoscedasticity, and normality of residuals.

## Dataset

The dataset contains information on:
- **Price**: Vehicle price in GBP.
- **Miles Driven**: Total mileage of the car.
- **Engine Power**: Power in BHP/PS.
- **Registration Year**: Year the vehicle was registered.

### Data Summary:
| Feature         | Count | Mean      | Std Dev   | Min   | Max    |
|-----------------|-------|-----------|-----------|-------|--------|
| Price (£)       | 100   | 32,393.97 | 8,103.81  | 10,995| 47,994 |
| Miles Driven    | 100   | 36,873.43 | 30,500.62 | 1,200 | 174,000|
| Engine Power    | 100   | 172.08    | 26.94     | 146   | 208    |
| Registration Yr | 100   | 2020      | 1.44      | 2018  | 2022   |

## Methodology

1. **Data Preprocessing**:
   - Converted engine power from text to numeric values.
   - Filtered data for vehicles registered between 2018-2022 to avoid outliers.
2. **Statistical Techniques**:
   - Confidence interval estimation for pricing.
   - Hypothesis testing for pricing across mileage groups.
   - Correlation analysis of price with engine power, mileage, and registration year.
3. **Regression Modeling**:
   - Multiple linear regression to predict vehicle prices:
     - **Dependent Variable**: Price.
     - **Independent Variables**: Miles driven, registration year, engine power.
   - Residual analysis to validate model assumptions.

### Regression Model Equation:
- Price = -4,849,000 - 0.1119 * Miles Driven + 2412.5954 * Registration Year + 68.1277 * Engine Power

## Results

- **Correlation Insights**:
  - Strong negative correlation between price and miles driven (-0.77).
  - Strong positive correlation between price and registration year (0.84).
  - Moderate positive correlation between price and engine power (0.69).
- **Model Accuracy**:
  - R²: 0.851, explaining 85.1% of the variance in pricing.
  - Prediction Example:
    - For a car with 30,000 miles driven, registered in 2020, and 150 BHP engine power:
      - **Predicted Price**: £31,304.86.

## Contributions
 - Contributions are welcome! Fork the repository, create a branch, and submit a pull request.
