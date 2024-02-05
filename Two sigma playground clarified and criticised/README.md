# Project Title: Two Sigma Financial Modeling

## Overview
This project focuses on the Two Sigma Financial Modeling competition hosted on Kaggle. The competition challenges participants to predict future stock market returns based on provided market and trading data.

## Project Structure
- **File Descriptions:**
  - `TwoSigma_Financial_Modeling.ipynb`: Jupyter notebook containing the main code for data preprocessing, feature engineering, model training, and prediction generation.
  - `README.md`: Project documentation providing an overview, file descriptions, and instructions.
  
- **Data:**
  - `train.h5`: Historical training data provided by Kaggle.
  - `test.h5`: Test data for prediction.
  
- **Code Libraries:**
  - `kagglegym`: Kaggle Gym API for interacting with the competition environment.
  - `numpy`: Library for numerical operations.
  - `pandas`: Data manipulation library.
  - `sklearn`: Machine learning library for model building.
  - `gc`: Garbage collection module for memory management.

- **Scripts/Functions:**
  - `fast_BaggingRegressor`: Custom bagging regressor for combining linear models efficiently.
  - `train_base_model_cv`: Cross-validated model training function.
  - `process_features_training`: Function for feature engineering during training.
  - `process_features_online`: Function for feature engineering during online prediction.
  
## Instructions
1. Run the `TwoSigma_Financial_Modeling.ipynb` notebook sequentially.
2. Ensure all required libraries are installed (`kagglegym`, `numpy`, `pandas`, `sklearn`).
3. Update file paths if necessary.
4. Execute the code cells to preprocess data, engineer features, train models, and generate predictions.
5. Review the results and the public score obtained on Kaggle.

## Notes
- The project uses a combination of linear models and custom bagging for improved prediction accuracy.
- Feature engineering involves creating rolling averages and differences for certain columns.
- The code is structured for both training and online prediction phases.

## Kaggle Competition Link
[Tow Sigma Financial Modeling Challenge](https://www.kaggle.com/c/two-sigma-financial-modeling)
