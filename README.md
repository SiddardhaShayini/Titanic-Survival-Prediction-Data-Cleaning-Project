# House Price Prediction Model

A simple machine learning project that predicts house prices using **Linear Regression**.

## Overview

This project:

* Loads a house price dataset from a CSV file.
* Selects numeric features for training.
* Handles missing numeric values.
* Splits the dataset into training and testing sets.
* Trains a Linear Regression model.
* Predicts house prices.
* Evaluates the model using the **R² score**.
* Visualizes predicted prices against actual prices.

## Requirements

Install the required Python libraries:

```bash
pip install pandas scikit-learn matplotlib seaborn
```

If you are using **Google Colab**, these libraries are usually already available.

## Dataset

Upload a CSV file containing a target column named:

```text
price
```

The model automatically selects numeric columns as input features.

Example:

```text
area, bedrooms, bathrooms, age, price
1200, 3, 2, 10, 250000
1500, 4, 2, 5, 320000
```

## How to Run

1. Open the notebook in Google Colab.
2. Run the dataset loading section.
3. Upload your CSV file when prompted.
4. Make sure your target column is named `price`.
5. Run the remaining cells.
6. Check the **R² score** and prediction graph.

## Model

The project uses:

**Linear Regression**

The data is split into:

* **80%** training data
* **20%** testing data

A `random_state` of `42` is used to make the split reproducible.

## Evaluation

The model is evaluated using the **R² (R-squared) score**.

An R² score closer to **1.0** generally indicates that the model explains more of the variation in house prices.

## Visualization

The project creates a scatter plot comparing:

* **Actual House Prices**
* **Predicted House Prices**

The red dashed line represents perfect predictions.

## Project Structure

```text
House-Price-Prediction/
│
├── house_price_prediction.ipynb
├── README.md
└── dataset.csv
```

## Limitations

This is a simple model intended for learning purposes.

* Only numeric columns are used.
* Categorical columns are ignored.
* Missing numeric values are filled with the mean.
* No advanced feature engineering is performed.
* Linear Regression may not work well for complex house-price relationships.

## Future Improvements

* Add categorical feature encoding.
* Try models such as Random Forest and Gradient Boosting.
* Perform feature engineering.
* Add more evaluation metrics such as MAE and RMSE.
* Tune model parameters.
