
# Smart Home Energy Consumption Prediction

## Project Overview

This project involves analyzing and predicting energy consumption in smart homes using different regression models. The objective is to evaluate and compare the performance of Linear Regression, Ridge Regression, and ElasticNet models to understand their effectiveness in predicting energy usage and determining feature importance.

## Dataset

The dataset used for this analysis contains various features related to energy consumption in smart homes. Key features include:
- **Temperature_C**: Temperature in Celsius.
- **Humidity_%**: Humidity percentage.
- **HVAC_Usage_kWh**: Energy usage by HVAC systems in kWh.
- **Kitchen_Usage_kWh**: Energy usage in the kitchen in kWh.
- **Electronics_Usage_kWh**: Energy usage by electronics in kWh.
- **7_day_MA**: 7-day moving average of energy consumption.
- **30_day_MA**: 30-day moving average of energy consumption.
- **Energy_per_Occupant_kWh**: Energy consumption per occupant in kWh.
- **Temperature_Difference_C**: Difference in temperature in Celsius.
- **Occupancy**: Binary feature indicating occupancy status.

## Models

Three regression models are implemented and evaluated:
1. **Linear Regression**: A basic regression model used as a baseline.
2. **Ridge Regression**: A regularized linear model to address potential overfitting.
3. **ElasticNet**: A model that combines L1 and L2 regularization to balance both regularization techniques.

## Evaluation Metrics

The models are evaluated using the following metrics:
- **Mean Absolute Error (MAE)**: Average absolute difference between predicted and actual values.
- **Mean Squared Error (MSE)**: Average squared difference between predicted and actual values.
- **Root Mean Squared Error (RMSE)**: Square root of the mean squared error.
- **R-squared (R²)**: Proportion of variance explained by the model.

## Results

### Model Evaluation Metrics
- **Linear Regression**:
  - MAE: 0.05
  - MSE: 0.01
  - RMSE: 0.09
  - R²: 0.7385
- **ElasticNet**:
  - MAE: 0.05
  - MSE: 0.01
  - RMSE: 0.09
  - R²: 0.7386
- **Ridge Regression**:
  - MAE: 0.05
  - MSE: 0.01
  - RMSE: 0.09
  - R²: 0.7361

### Conclusion
- **ElasticNet** has the highest R² value, indicating it explains the most variance in the target variable.
- **Linear Regression** and **Ridge Regression** show similar performance, with Linear Regression being nearly as effective as ElasticNet.
- **Ridge Regression** provides a good balance between simplicity and performance.

ElasticNet is recommended for its slightly better R² value, but Linear Regression and Ridge Regression are also strong candidates depending on the need for regularization and model complexity.

## Installation

To run the Jupyter Notebook and reproduce the results, ensure you have the necessary Python packages installed. You can install them using the `requirements.txt` file:

```bash
pip install -r requirements.txt
