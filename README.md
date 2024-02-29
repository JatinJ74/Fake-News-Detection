# Fake News Detection using NLP and Machine Learning

## Overview

This Python script is designed to detect fake news articles using Natural Language Processing (NLP) techniques and machine learning algorithms. The script preprocesses the text data, applies TF-IDF vectorization, and trains multiple classification models to classify news articles as fake or real. It evaluates the performance of the models and provides insights into the accuracy of the predictions.

## Features

- Utilizes NLP techniques for text preprocessing and feature extraction.
- Implements multiple machine learning models, including Passive Aggressive Classifier and Naive Bayes, for classification.
- Evaluate model performance using accuracy score, confusion matrix, and classification report.
- Provides a function to test the model on real-time news articles.

## Usage

1. **Clone the Repository**: 
    ```
    git clone <repository_url>
    ```

2. **Install Dependencies**:
    ```
    pip install -r requirements.txt
    ```

3. **Run the Script**:
    ```
    python fake_news_detection.py
    ```

4. **Input News Articles**:
    - Provide news articles as input to the script.
    - The script will classify each news article as fake or real based on the trained models.

## Dataset

The script uses a dataset of labeled news articles for training and testing. The dataset is stored in a CSV file named `news.csv` and contains two columns: `text` (news article text) and `label` (fake or real).

## Model Training and Evaluation

- The script splits the dataset into training and testing sets using a specified test size.
- It preprocesses the text data, applies TF-IDF vectorization, and trains multiple classification models.
- It evaluates the performance of each model using an accuracy score, confusion matrix, and classification report.
- The best-performing model is saved as a pickle file named `model.pkl` for future use.

## Testing Real-Time News

- The script provides a function `fake_news_det(news)` to test the trained model on real-time news articles.
- Input a news article as a string to the function, and it will classify the article as fake or real.

