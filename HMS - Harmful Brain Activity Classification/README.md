# Brain Activity Classification with EEG Spectrograms

This project aims to classify brain activity using EEG (Electroencephalogram) spectrograms. The goal is to develop a deep learning model that can accurately identify different types of brain activity from EEG data.

## Overview

The project consists of the following main components:
- Data preprocessing: EEG spectrograms in .parquet format are converted to .npy format for easier loading and processing. Spectrograms are then preprocessed and augmented for training.
- Model training: A deep neural network model is trained using the preprocessed spectrogram data. The model architecture is based on EfficientNetV2 B2, pretrained on ImageNet, and fine-tuned for the classification task.
- Evaluation: The trained model is evaluated using stratified k-fold cross-validation. Metrics such as KL Divergence loss are used to assess model performance.
- Inference: The best performing model is used to make predictions on unseen test data.
- Submission: Predictions are formatted and submitted for evaluation in the competition.

## Requirements

- Python 3.x
- TensorFlow
- Keras
- Pandas
- NumPy
- OpenCV
- Joblib
- Matplotlib
- Seaborn

## Usage

1. Clone the repository:

```
git clone https://github.com/awrsha/HMS - Harmful Brain Activity Classification.git
```

2. Navigate to the project directory:

```
cd HMS - Harmful Brain Activity Classification
```

3. Run the preprocessing script to convert .parquet files to .npy format:

```
hms-hbac-kerascv-starter-notebook-e280b3.ipynb
```


## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
