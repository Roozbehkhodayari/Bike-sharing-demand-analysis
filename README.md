# Bike Sharing Demand Analysis and Prediction

## Overview

This project explores the Bike Sharing Dataset to better understand the factors associated with bike rental demand.

The analysis includes:

* Data cleaning and preparation
* Exploratory data analysis (EDA)
* Numerical and categorical visualizations
* Grouped analysis and trend analysis
* Feature engineering
* Linear Regression modeling
* Model evaluation and interpretation

The project was completed as part of the DX602 course and is designed as both a final submission and a portfolio project.

---

## Project Structure

1. Introduction
2. Load and Inspect the Data
3. Data Cleaning and Preparation
4. Descriptive Statistics
5. Numerical Visualizations
6. Categorical Analysis
7. Grouped Analysis
8. Feature Engineering
9. Trends Over Time
10. Variable Relationships
11. Hypothesis
12. Linear Regression
13. Reflection / Conclusion

---

## Dataset Features

The dataset includes variables related to:

* Weather conditions
* Temperature and humidity
* Time and seasonal patterns
* Working days and holidays
* Bike rental counts

Target variable:

* `count` → total number of bike rentals

---

## Feature Engineering

Several engineered features were created during the project, including:

* `peak_period`
* Cyclical hour features:

  * `hour_sin`
  * `hour_cos`

These features helped better represent daily rental behavior and cyclical time patterns.

---

## Modeling

A Linear Regression model was built to predict bike rental demand.

### Preprocessing Steps

* Dummy encoding for categorical variables
* Scaling of numerical variables
* Removal of highly correlated or leakage-related variables
* Cyclical encoding of hour values

### Model Performance

| Metric   | Value   |
| -------- | ------- |
| MSE      | 8700.82 |
| RMSE     | 93.28   |
| R² Score | 0.7364  |

The model explains a substantial portion of the variation in bike rental demand, although prediction errors remain for some higher rental values.

---

## Main Insights

* Time-related variables are strongly associated with rental demand.
* Rental activity changes across weather conditions and seasons.
* Working-day commuting patterns create clear peaks in demand.
* Linear Regression captures general trends reasonably well but struggles with more complex non-linear behavior.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

## Repository Contents

* `bike-sharing-demand-analysis.ipynb` → main notebook
* `README.md` → project overview and documentation

---

## Future Improvements

Potential future improvements include:

* Using tree-based models such as Random Forest or XGBoost
* Additional feature engineering
* Hyperparameter tuning
* Improved handling of extreme rental values

---

## Author

Roozbeh Khodayari
