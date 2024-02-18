# Rossmann Store Sales Prediction

This project focuses on predicting the sales of Rossmann stores using historical data. The dataset contains information about the stores, such as their promotions, competitors, and other factors that might influence sales. The goal is to build a predictive model that can accurately forecast sales based on these features.

## Table of Contents

1. [Introduction](#introduction)
2. [Data](#data)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Conclusion](#conclusion)
6. [Usage](#usage)
7. [Dependencies](#dependencies)
8. [Contributing](#contributing)
9. [License](#license)

## Introduction

Rossmann operates over 3,000 drug stores in 7 European countries. The data provided contains historical sales data for 1,115 Rossmann stores. The goal of this project is to predict future sales using this historical data, taking into account various factors such as promotions, competition, and school holidays.

## Data

The dataset consists of several CSV files:

- `train.csv`: Contains historical sales data for Rossmann stores.
- `store.csv`: Provides additional information about each store.
- `test.csv`: Contains data for which predictions are to be made.
- `sample_submission.csv`: A sample submission file in the correct format.

## Methodology

1. **Data Preprocessing**: The data is loaded and cleaned. Missing values are handled appropriately, and the features are prepared for modeling.

2. **Exploratory Data Analysis (EDA)**: Various visualizations are used to understand the relationships between different variables and the target variable (sales).

3. **Modeling**: Two approaches are explored for modeling:
   - Simple Neural Network: A basic neural network model is trained using Keras.
   - Long Short-Term Memory (LSTM): A more complex model suitable for time series data is implemented using LSTM.

4. **Evaluation**: The models are evaluated based on their performance metrics such as R-squared score.

## Results

- The Simple Neural Network achieved an R-squared score of 0.718 on the training set and 0.472 on the test set.
- The LSTM model's performance will be added here once completed.

## Conclusion

This project demonstrates the feasibility of predicting Rossmann store sales using historical data and machine learning models. The models developed can help Rossmann make informed decisions about inventory, staffing, and promotions to optimize sales.

## Usage

To use this project:

1. Clone the repository: `git clone https://github.com/username/rossmann-store-sales.git`
2. Run the main script: `python Rossman-Store-Sales.ipynb`

## Dependencies

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- TensorFlow
- Keras
- Scikit-learn
- Statsmodels

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
