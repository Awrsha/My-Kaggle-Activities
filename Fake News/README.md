# Fake News Classification using Support Vector Machines (SVM)

## Overview

This project focuses on building a fake news classification model using Support Vector Machines (SVM). The dataset used for training and testing the model is obtained from Kaggle and consists of labeled news articles.

## Dataset

The dataset contains labeled news articles with columns such as 'id,' 'title,' 'author,' 'text,' and 'label.' The 'label' column indicates whether the news is real (0) or fake (1).

Download the data file from here : [Link](https://www.kaggle.com/competitions/fake-news)

## Data Preprocessing

- Merged 'author' and 'title' columns to create a new feature.
- Cleaned and preprocessed the text data by removing non-alphabetic characters, converting to lowercase, and applying stemming.
- Utilized TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to convert text data into numerical features.

## Model Training

- Implemented a Support Vector Machines (SVM) model with a linear kernel.
- Trained the model on the preprocessed training data.

## Prediction

- Applied the trained SVM model to make predictions on the test data.
- Saved the predictions in a CSV file named 'submission.csv.'

## Repository Contents

- **Notebooks**: Jupyter notebook containing code for data preprocessing, model development, and predictions.
- **Data**: Folder containing the train and test datasets.
- **Models**: Folder containing the saved SVM model weights.
- **Readme.md**: Documentation file providing an overview of the project, instructions, and key findings.
- **Submission.csv**: CSV file containing the predictions for the test data.

## Instructions

1. Clone the repository: `git clone <repository_url>`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Execute the Jupyter notebook in the `Notebooks` directory to run the project.
4. View the predictions in the 'Submission.csv' file.

## Results

- The SVM model achieved predictions on the test set, saved in the 'Submission.csv' file.
