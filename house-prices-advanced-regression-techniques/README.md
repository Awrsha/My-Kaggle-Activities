# House Prices Prediction Project

## Overview

This project focuses on predicting house prices using advanced regression techniques. The dataset is sourced from the Kaggle competition "House Prices: Advanced Regression Techniques." The goal is to develop a predictive model that can accurately estimate the sale prices of houses.

## Dataset

- **train.csv**: Contains the training data with features and target variable.
- **test.csv**: Consists of the test data for making predictions.

Download the data file from here : [Link](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
  
## Data Exploration and Preprocessing

- The project starts with loading and exploring the dataset.
- Initial analysis, including statistical summaries and visualization, is performed.
- Data preprocessing steps involve handling missing values, log-transforming the target variable, and creating additional features.

## Feature Engineering

- Several features are created to enhance the predictive power of the model.
- New variables like `SqFtPerRoom`, `Total_Home_Quality`, `Total_Bathrooms`, and `HighQualSF` are introduced.

## Model Development

- The main machine learning algorithm used is XGBoost with hyperparameter tuning.
- Cross-validation is applied to ensure the robustness of the model.
- A Randomized Search approach is utilized for hyperparameter optimization.

## Evaluation

- The performance of the model is evaluated using Root Mean Squared Error (RMSE) as the metric.
- A detailed analysis of the cross-validation results is provided.

## Prediction and Submission

- The trained model is used to predict house prices for the test dataset.
- Predictions are transformed back to the original scale (if log-transformed).
- The results are saved in a submission file (`submission.csv`) for Kaggle.

## Repository Contents

- **Notebooks**: Jupyter notebooks containing code for data exploration, preprocessing, and modeling.
- **Data**: Folder containing the training and test datasets.
- **Submission**: Folder containing the final submission file.
- **Readme.md**: Documentation file providing an overview of the project, instructions, and key findings.

## Instructions

1. Clone the repository: `git clone <repository_url>`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Execute the Jupyter notebooks in the `Notebooks` directory in sequential order.
4. Review the `submission.csv` file for the final predictions.

## Results

- The model achieves competitive results with an RMSE of [0.141, 0.162, 0.204, 0.197, 0.157] during cross-validation.
- The submission file (`submission.csv`) is ready for upload to the Kaggle competition.
