# Email/SMS Spam Classifier

This project is a web-based application that classifies whether a given message is spam or not. The application is built using Streamlit for the front-end and a trained machine learning model for the classification task.

## Features

- Takes an input message from the user
- Preprocesses the message (removal of stop words, punctuation, and stemming)
- Classifies the message as **Spam** or **Not Spam**
- Displays the classification result on the web interface

## Tech Stack

- **Python**: Core language used for the project
- **Streamlit**: Framework for building the web interface
- **Numpy, Pandas, NLTK**: Libraries for text preprocessing and transformations
- **Scikit-learn**: Used for building the ML model
- **Pickle**: Used for loading the pre-trained model and TF-IDF vectorizer

## How It Works

1. **Text Preprocessing**: The input message is converted to lowercase, tokenized, and filtered to remove stopwords and punctuation. Then, the tokens are stemmed using the PorterStemmer.
   
2. **Vectorization**: After preprocessing, the message is transformed into a TF-IDF vector using a pre-trained vectorizer.

3. **Prediction**: The model predicts whether the message is spam or not based on the TF-IDF vector.

4. **Result Display**: The result is shown on the web interface as "Spam" or "Not Spam".

