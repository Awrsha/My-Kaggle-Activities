# House Rent Prediction Project

This repository contains the code and data for a project focused on predicting house rent based on various features. The project includes data visualization, data preprocessing, and the application of different regression models, including linear regression, support vector machine (SVM), random forest, XGBoost, and ridge regression. Additionally, a neural network model is implemented using TensorFlow and Keras.

## Dataset

The dataset used for this project is sourced from Kaggle and is named `houses_to_rent.csv`. It contains information about houses, including features like city, area, number of rooms, bathrooms, parking spaces, floor, and various financial attributes such as rent amount, property tax, fire insurance, and total cost.
download dataset file here : [Link](https://www.kaggle.com/datasets/antonyroy/finaltry)

## Data Visualization

The project includes sample plots using Seaborn and Matplotlib to visualize relationships between different variables, distribution of rent amount in different cities, and the impact of furniture presence on rent.

## Data Preprocessing

Data preprocessing steps include handling missing values, removing rows with invalid data in the 'floor' column, and one-hot encoding categorical variables like 'city', 'animal', and 'furniture'.

## Model Training and Evaluation

Several regression models are trained and evaluated using the Scikit-learn library. The models include Linear Regression, Support Vector Machine Regressor, Random Forest Regressor, XGBoost Regressor, and Ridge Regression. Cross-validation is used to assess model performance.

## Neural Network Model

A neural network model is implemented using TensorFlow and Keras. The model is trained on scaled data, and its performance is evaluated using mean squared error and mean absolute error.

## Example Prediction

An example of predicting rent for new data is included using the trained linear regression model.

## File Structure

- `data/`: Contains the dataset used in the project.
- `notebooks/`: Jupyter notebooks with code for data analysis and model implementation.
- `README.md`: Documentation providing an overview of the project.

## Usage

To run the project, follow these steps:

1. Clone the repository to your local machine.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Run the Jupyter notebooks in the `notebooks/` directory in the specified order.

## Dependencies

The project uses the following Python libraries:

- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn
- xgboost
- tensorflow

## Acknowledgments

- Kaggle for providing the dataset.

Feel free to explore and modify the code to suit your needs. If you have any questions or suggestions, please open an issue or contact the project contributors.
