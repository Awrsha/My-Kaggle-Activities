# Flower Classification using Convolutional Neural Network (CNN)

## Overview

This project focuses on building a Convolutional Neural Network (CNN) to classify images of flowers into five different categories. The dataset used is the "5 Flower Types Classification Dataset" from Kaggle. The CNN is developed using TensorFlow and Keras.

## Dataset

The dataset consists of images of flowers categorized into five classes. The images are split into training, testing, and validation sets.

Download the data file from here : [Link](https://www.kaggle.com/datasets/kausthubkannan/5-flower-types-classification-dataset)

## Data Preprocessing

- Images are loaded and labeled from the dataset.
- Data is split into training, testing, and validation sets.
- ImageDataGenerator is used for data augmentation during training.

## Model Architecture

- A CNN model is built using TensorFlow and Keras.
- The architecture includes Conv2D layers, MaxPooling layers, Flatten layer, and Dense layers.
- The model is compiled using the Adam optimizer and categorical crossentropy loss function.

## Training

- The model is trained on the training set with augmentation.
- Validation data is used to monitor the model's performance during training.
- The training process involves 100 epochs.

## Evaluation

- The trained model is evaluated on the test set to assess its accuracy.
- Evaluation results include loss and accuracy metrics.

## Repository Contents

- **Notebooks**: Jupyter notebook containing code for data preprocessing, model development, and training.
- **Data**: Folder containing the flower images dataset.
- **Models**: Folder containing the saved model weights.
- **Readme.md**: Documentation file providing an overview of the project, instructions, and key findings.

## Instructions

1. Clone the repository: `git clone <repository_url>`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Execute the Jupyter notebook in the `Notebooks` directory to run the project.
4. Review the model's performance on the test set.

## Results

- The CNN achieves an accuracy of approximately 81.33% on the test set.
- Model weights are saved in the `Models` folder for future use.
