# Diabetes Prediction

This project aims to predict the occurrence of diabetes using machine learning techniques. The dataset used for this analysis is the "diabetes_prediction_dataset.csv" file, which contains various features related to an individual's health condition.

## Data Preprocessing

1. The dataset is loaded into a Pandas DataFrame.
2. A random sample of 1000 instances is selected from the initial dataset.
3. Categorical features like 'gender' and 'smoking_history' are label-encoded.
4. The target variable 'diabetes' is separated from the feature variables.
5. The Synthetic Minority Over-sampling Technique (SMOTE) is applied to balance the target variable classes.
6. A correlation heatmap is generated to visualize the relationships between features.
7. The age feature is binned into groups for better visualization.
8. Feature scaling is performed using StandardScaler.

## Model Building and Evaluation

1. A grid search is performed to find the optimal hyperparameters for Random Forest and AdaBoost classifiers.
2. The feature importances of the Random Forest model are visualized.
3. The dataset is split into training and testing sets.
4. Several machine learning models are trained and evaluated on the test set:
  - Random Forest Classifier
  - Logistic Regression
  - AdaBoost Classifier
  - Decision Tree Classifier
  - Gradient Boosting Classifier
5. Performance metrics like accuracy, precision, recall, and F1-score are calculated for each model.
6. The Receiver Operating Characteristic (ROC) curve and Area Under the Curve (AUC) are plotted for the Gradient Boosting Classifier.
7. A simple neural network is trained and evaluated on the dataset.

## Model Deployment

1. A new data point is defined for prediction.
2. The new data is scaled using the same scaler as the training data.
3. The trained Gradient Boosting Classifier model predicts the probability of diabetes for the new data point.

## Usage

To run this project, you'll need to have the following dependencies installed:

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn
- TensorFlow (for the neural network part)

You'll also need to have the 'diabetes_prediction_dataset.csv' file in the same directory as your Python script.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.