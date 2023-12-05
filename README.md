# ML Spam Detector

This project includes a simple machine learning model to classify text messages as spam or not spam (ham). It utilizes Python's data analysis library `pandas`, numerical library `numpy`, and several components from the machine learning library `scikit-learn`.

## Dataset

The dataset used for training the classifier is a collection of text messages that have been labeled as 'ham' or 'spam'. The data is read from a CSV file and preprocessed for the classification task.

## Dependencies

- pandas
- numpy
- scikit-learn

You can install these dependencies via `pip`:

pip install pandas numpy scikit-learn

## Data Preparation
The messages from the dataset are converted into a format that can be fed into a machine learning model, using a CountVectorizer for text vectorization, which turns the text messages into a matrix of token counts.

## Model Training
A MultinomialNB (Multinomial Naive Bayes) classifier is trained on the processed data. This classifier is particularly suited for classification with discrete features (like word counts for text classification).

## Usage
After training, the model can predict whether a new message is spam. An example usage is provided that allows a user to enter a message and receive a classification result.
