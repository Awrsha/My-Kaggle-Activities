
1. **Data Loading and Preprocessing:**
   - You loaded the training and test datasets using Pandas.
   - You separated labels and features and created training and validation sets.
   - Normalized pixel values to the range [0, 1].
   - Reshaped the datasets to have a 4D shape suitable for CNN input.

2. **Label Encoding:**
   - Converted the categorical labels into one-hot encoded vectors.

3. **CNN Model Architecture:**
   - Built a Sequential model using Keras.
   - Added Conv2D layers with activation (elu) and dropout for regularization.
   - Added MaxPooling2D layers for downsampling.
   - Flattened the output and added Dense layers with dropout.
   - Output layer with 10 neurons (for each digit) using the sigmoid activation function.

4. **Model Compilation:**
   - Used Stochastic Gradient Descent (SGD) as the optimizer.
   - Compiled the model with categorical cross-entropy loss and accuracy as the metric.

5. **Callbacks:**
   - Utilized EarlyStopping, ReduceLROnPlateau, and ModelCheckpoint callbacks to monitor training progress.

6. **Model Training:**
   - Trained the model on the training set for 30 epochs.
   - Monitored validation loss for early stopping and learning rate reduction.

7. **Model Evaluation:**
   - Evaluated the model on the validation set.

8. **Prediction:**
   - Used the trained model to predict labels for the test set.

9. **Submission:**
   - Created a submission file with the predicted labels in the required format.

10. **Note:**
    - You received a convergence warning during logistic regression training, suggesting potential issues with convergence. It's advisable to explore options like increasing the number of iterations or scaling the data.
