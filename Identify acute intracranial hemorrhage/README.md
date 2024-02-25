# RSNA Intracranial Hemorrhage Detection Project

## Introduction
This project aims to develop a model for the detection of intracranial hemorrhage (ICH) using medical imaging data provided by the Radiological Society of North America (RSNA). Intracranial hemorrhage is a critical condition that requires prompt diagnosis and treatment to prevent serious consequences. The dataset consists of DICOM images containing various types of intracranial hemorrhage, including epidural, subdural, subarachnoid, intraparenchymal, intraventricular, and any. 

## Project Structure
- **Data Preprocessing**: The DICOM images are preprocessed to apply windowing techniques, correct pixel values, and prepare them for model input.
- **Model Development**: A deep learning model is developed using TensorFlow/Keras to classify DICOM images into different types of intracranial hemorrhage.
- **Evaluation**: Model performance is evaluated using appropriate evaluation metrics such as weighted log loss and validation accuracy.
- **Visualization**: Visualizations are generated to understand the distribution of labels and the effectiveness of windowing techniques in enhancing image features.
- **Readme.md**: This document provides an overview of the project, its structure, and relevant information.

## Data Preprocessing
- DICOM images are read and processed using the PyDICOM library.
- Windowing techniques are applied to enhance features relevant to brain, subdural, and soft tissue windows.
- Pixel values are corrected as necessary to ensure accurate representation of image intensity.

## Model Development
- A deep learning model is developed using transfer learning with a pre-trained architecture (e.g., ResNet, DenseNet) to classify intracranial hemorrhage.
- The model is trained using the processed DICOM images and evaluated using appropriate evaluation metrics.
- Custom loss functions and metrics are implemented to account for class imbalance and optimize model performance.

## Evaluation
- Model performance is evaluated using metrics such as weighted log loss and validation accuracy.
- Cross-validation or train-validation splits are employed to assess the generalization ability of the model.
- Results are analyzed to identify areas for improvement and fine-tuning.

## Visualization
- Visualizations are generated to explore the distribution of labels in the dataset.
- Sample DICOM images are visualized before and after windowing to demonstrate the effectiveness of preprocessing techniques.

## Usage
- Clone the repository.
- Ensure all dependencies are installed as specified in the requirements file.
- Follow the instructions in the project scripts to preprocess data, train the model, and evaluate performance.
- Refer to the readme.md for detailed instructions and usage guidelines.

## Conclusion
This project demonstrates the application of deep learning techniques for the detection of intracranial hemorrhage using medical imaging data. By preprocessing DICOM images and developing a robust classification model, accurate and timely diagnosis of this critical condition can be achieved, potentially improving patient outcomes.
