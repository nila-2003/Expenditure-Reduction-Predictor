# Expenditure Reduction Predictor

This project is aims at predicting the total expenditure for an event based on the prices provided by various vendors, and visualizing areas where expenditure can be reduced to meet the initial budget.

## Overview

The Expenditure Reduction Predictor utilizes a machine learning model trained on historical data to predict the total expenditure for an event. It takes into account the initial budget and the prices provided by vendors in different categories such as decor, bakery, catering, and music. The model can then be called to be used in the function for calculating the amounts.

If the predicted total expenditure exceeds the initial budget, the system identifies areas where expenditure can be reduced by suggesting ideal rates for each vendor category.

## Features

- Predicts total expenditure based on vendor prices and initial budget.
- Visualizes areas where expenditure can be reduced if the predicted total expenditure exceeds the initial budget.
- Provides breakdown of expenses including vendor prices and total predicted expenditure.

## Usage

To use the Expenditure Reduction Predictor, follow these steps:

1. Install the required dependencies by running `pip install -r requirements.txt`.
2. Prepare your dataset in CSV format with columns: 'Initial Price', 'Vendor Category', 'Vendor Price', 'Final Price'.
3. Run the `predict_and_visualize` function with your initial budget and vendor details as input.

## Example

```python
initial_budget = 300.00
vendor_details = {
    'decor': 20.00,
    'music': 100.00,
    'bakery': 20.00
}
predict_and_visualize(initial_budget, vendor_details)
