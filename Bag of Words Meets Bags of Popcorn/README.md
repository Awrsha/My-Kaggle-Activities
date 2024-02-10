# Sentiment Analysis with Word2Vec

## Overview
This project aims to perform sentiment analysis on movie reviews using Word2Vec embeddings. The dataset used for this analysis includes labeled movie reviews from the IMDb website. The analysis involves preprocessing the text data, training a Word2Vec model to generate word embeddings, and using these embeddings to create document vectors for sentiment classification. Finally, various machine learning classifiers are trained on the document vectors to predict the sentiment of movie reviews.

## Dataset
The dataset used in this project consists of labeled movie reviews sourced from the IMDb website. It contains three main components:
- **labeledTrainData.tsv.zip:** This file contains labeled training data with 25,000 movie reviews, each labeled as either positive or negative sentiment.
- **testData.tsv.zip:** This file contains 25,000 unlabeled test data points for which sentiment needs to be predicted.
- **imdb_master.csv:** An additional dataset containing 50,000 labeled movie reviews, which includes both positive and negative sentiments.

## Preprocessing
1. **Data Cleaning:** The text data undergoes several cleaning steps, including the removal of HTML tags, URLs, special characters, digits, and extra white spaces.
2. **Normalization:** Text data is converted to lowercase, and accents and emojis are removed.
3. **Tokenization:** Movie reviews are tokenized into individual words for further processing.
4. **Word Filtering:** Words shorter than one character are removed from the tokenized text.

## Word2Vec Model Training
A Word2Vec model is trained on the preprocessed movie review data to generate word embeddings. The parameters used for training the Word2Vec model include feature size, context size, minimum word count, and number of epochs.

## Document Vector Creation
Document vectors are created by taking the mean of word vectors for each document. These document vectors serve as features for sentiment classification.

## Model Training and Evaluation
Several machine learning classifiers are trained on the document vectors to predict the sentiment of movie reviews. The classifiers used include:
- Random Forest Classifier
- Gradient Boosting Classifier
- Decision Tree Classifier
- Logistic Regression
- K-Nearest Neighbors Classifier
- Gaussian Naive Bayes Classifier
- Bernoulli Naive Bayes Classifier
- XGBoost Classifier
- Multinomial Naive Bayes Classifier

The trained models are evaluated using metrics such as accuracy, precision, recall, and F1-score. The best-performing model is then used to make predictions on the test data.

## Submission
A submission file containing the predicted sentiments for the test data is created and saved in CSV format.

## File Structure
The project files are organized as follows:
- **README.md:** This file provides an overview of the project, dataset, preprocessing steps, model training, evaluation, and submission details.
- **Code File:** Contains the Python code for preprocessing, model training, evaluation, and prediction.
- **Dataset Folder:** Contains the input data files used for training and testing.
- **Submission Folder:** Contains the submission file with predicted sentiments for the test data.

## Instructions for Running the Code
1. Download or clone the repository to your local machine.
2. Ensure you have Python installed along with necessary libraries mentioned in the code.
3. Run the code file to preprocess the data, train the models, and generate predictions.
4. The submission file will be created in the submission folder.

## Acknowledgments
- The dataset used in this project is sourced from IMDb and made available through Kaggle.
- Various Python libraries such as Pandas, NumPy, NLTK, Gensim, Scikit-learn, and Keras are used for data manipulation, text preprocessing, model training, and evaluation.

## Author
[Amir M Parvizi]

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## References
- [Kaggle](https://www.kaggle.com/)
- [IMDb](https://www.imdb.com/)
- [Word2Vec Tutorial](https://www.kaggle.com/c/word2vec-nlp-tutorial)
