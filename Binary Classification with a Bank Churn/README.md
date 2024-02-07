# Kaggle Churn Prediction

This project involves predicting customer churn using a dataset provided by Kaggle. Customer churn is a critical metric for businesses, especially subscription-based services, as it directly impacts revenue and growth. The project utilizes machine learning techniques to build a predictive model.

## Environment

The project is implemented in Python 3 and utilizes various analytics libraries. The environment is defined by the `kaggle/python` Docker image. Key libraries used include:
- `numpy`: For numerical computations
- `pandas`: For data manipulation and analysis
- `scikit-learn`: For machine learning algorithms and evaluation metrics
- `catboost`: For gradient boosting implementation
- `shap`: For generating SHAP (SHapley Additive exPlanations) values for model interpretation

## Dataset

The dataset consists of multiple CSV files:
- `train.csv`: Training data containing features and churn labels
- `test.csv`: Test data for making predictions
- `sample_submission.csv`: Sample submission format for Kaggle competition

## Preprocessing

- Features such as `Age`, `CreditScore`, `Balance`, and `EstimatedSalary` are scaled to improve model performance.
- Additional features like `IsSenior`, `IsActive_by_CreditCard`, `Products_Per_Tenure`, `AgeCat`, and `Sur_Geo_Gend_Sal` are engineered based on domain knowledge and intuition.

## Model Training

- The model training process involves stratified k-fold cross-validation with CatBoostClassifier, which is a gradient boosting algorithm specifically optimized for categorical features and large datasets.
- AUC (Area Under the ROC Curve) is used as the evaluation metric.
- The final model is trained using GPU acceleration to expedite the process.

## SHAP Explanation

- SHAP values are calculated to explain the model predictions and understand the impact of each feature on the model's output.
- SHAP summary plots are generated to visualize the feature importance.

## Final Predictions

- The model predicts the probability of churn for the test dataset.
- Predictions are averaged across folds to improve robustness.

## Submission

- The predictions are saved in the required format (`submission.csv`) for submission to the Kaggle competition.

## Performance

The model achieves a mean AUC of approximately 0.8974 across the folds, indicating good predictive performance.

For more details, refer to the code implementation and comments provided in the project files.
