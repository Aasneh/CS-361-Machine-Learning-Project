# Improving Predictive Performance of GBoost and XGBoost Algorithms on Time Series Data Forecasting

This repository contains the project titled "Improving Predictive Performance of GBoost and XGBoost Algorithms on Time Series Data Forecasting by Working on Learning Rate," where we implemented and optimized Gradient Boosting and XGBoost algorithms for time series forecasting.

## Table of Contents

- [Brief Overview](#brief-overview)
- [Data Sources](#data-sources)
- [Model](#model)
- [Results and Evaluation](#results-and-evaluation)
- [Deployment](#deployment)
- [Conclusions and Further Improvements](#conclusions-and-further-improvements)

## Brief Overview
[(Back to top)](#table-of-contents)

This project investigates the application of Gradient Boosting and XGBoost for time series data forecasting, focusing on improving their predictive performance through learning rate optimization. Techniques such as Simulated Annealing and Adam Optimizer were used to fine-tune the learning rates.

### Key Techniques Used:
- **FFT Denoising:** Applied to remove noise from the time series data.
- **Simulated Annealing:** Used to adaptively adjust the learning rate.
- **Adam Optimizer:** Employed for adaptive learning rate optimization.
- **K-Fold Cross Validation:** Implemented to ensure model robustness and generalization.

## Data Sources
[(Back to top)](#table-of-contents)

The project utilizes the **Hourly Energy Consumption Dataset** from Kaggle for time series analysis. The dataset includes:

- **Timestamp:** Date and time of the energy consumption measurement.
- **Energy Consumption:** Measured in megawatts (MW).

[Link to Dataset](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption/data?select=PJME_hourly.csv)

## Model
[(Back to top)](#table-of-contents)

The model architecture is based on the principles of decision trees used in boosting algorithms. The project implements:

- **Gradient Boosting (GBoost):** Built with fixed, simulated annealing, and Adam-optimized learning rates.
- **Extreme Gradient Boosting (XGBoost):** Implemented with similar learning rate variations.

### Model Summary:
- **GBoost:** Enhanced using FFT Denoising, Simulated Annealing, and Adam Optimizer.
- **XGBoost:** Leveraged for its scalability and efficiency, with learning rate optimization.

## Results and Evaluation
[(Back to top)](#table-of-contents)

The model was evaluated using RMSE (Root Mean Square Error) and other metrics. Below are the comparison results for different configurations:

### RMSE Scores (GBoost vs XGBoost) on complete Dataset:
- **Fixed Learning Rate:** 
  - GBoost: 4335.07 
  - XGBoost: 3864.85
- **Simulated Annealing:** 
  - GBoost: 4237.27 
  - XGBoost: 3747.61
- **Adam Optimizer:** 
  - GBoost: 4126.99 
  - XGBoost: 3745.79

## Deployment
[(Back to top)](#table-of-contents)

The models are designed for easy deployment and can be tested using a Python environment. Future work may involve deploying these models via a web application.

## Conclusions and Further Improvements
[(Back to top)](#table-of-contents)

The project successfully implemented and optimized GBoost and XGBoost for time series forecasting. While our custom implementations outperformed standard library versions in accuracy, there is potential for further enhancement in computational efficiency.

### Future Enhancements:
- Implementing multi-threading for faster computations.
- Further refining node split computations to reduce training time.
