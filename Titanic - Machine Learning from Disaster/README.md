# Titanic Survival Prediction

## Overview

This repository contains code for predicting the survival of passengers on the Titanic using various machine learning models. The dataset used is sourced from the Titanic Kaggle competition. The project involves data preprocessing, exploration, and the application of three different models: Gradient Boosting, Neural Network, and Random Forest.

## Dataset

The dataset used for training the models is available in the `/kaggle/input/titanic/` directory. It includes features such as age, gender, class, and embarkation port.

Download the data file from here : [Link](https://www.kaggle.com/competitions/titanic)

## Models

### Gradient Boosting

A Gradient Boosting Classifier was trained using the `GradientBoostingClassifier` from scikit-learn. The model was evaluated on a test set, and predictions were saved in `gb_submission.csv`.

### Neural Network

A Neural Network model was implemented using Keras. It consists of three layers with ReLU activation in hidden layers and sigmoid activation in the output layer. The model was trained on resampled data using SMOTE to address class imbalance.

### Random Forest

A Random Forest Classifier was trained using the `RandomForestClassifier` from scikit-learn. The model was evaluated on a test set, and predictions were saved in `submission.csv`.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/your-username/titanic-survival-prediction.git
cd titanic-survival-prediction
```

2. Run the notebooks:

   - Open and run `Gradient_Boosting.ipynb` for the Gradient Boosting model.
   - Open and run `Neural_Network.ipynb` for the Neural Network model.
   - Open and run `Random_Forest.ipynb` for the Random Forest model.

3. Check the saved predictions:

   - `gb_submission.csv` for Gradient Boosting.
   - `submission.csv` for Random Forest.

## Dependencies

Ensure you have the required Python packages installed by running:

```bash
pip install -r requirements.txt
```

## License

This project is licensed under the [MIT License](LICENSE).
