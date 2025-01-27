Spam SMS Detection

Introduction

Unwanted spam messages are a major nuisance in modern communication systems. Spam SMS Detection is a crucial task to protect users from malicious links, fraudulent schemes, and irrelevant advertisements. This project focuses on building a machine learning model to classify SMS messages as either Spam or Ham (Not Spam).

By leveraging natural language processing (NLP) techniques and machine learning, the project aims to create an efficient system that can automatically filter spam messages, enhancing user experience and security.

About the Model

This project implements a machine learning pipeline to classify text messages. Below is an overview of the approach:

1. Dataset
The dataset used for this project is the popular SMS Spam Collection dataset, which contains:
5,574 SMS messages, labeled as "spam" or "ham."

Features: The message text is the primary feature, while the label represents the target classification.

2. Data Preprocessing

Since the dataset involves text, preprocessing steps include:

Text Cleaning: Remove punctuation, special characters, and stopwords.

Lowercasing: Convert all text to lowercase for uniformity.

Tokenization: Split messages into individual words.

Vectorization: Convert text into numerical form using:
Bag-of-Words (BoW)
TF-IDF (Term Frequency-Inverse Document Frequency)

3. Model Selection

Several machine learning algorithms were evaluated:

Naive Bayes: Ideal for text classification due to its simplicity and performance on small datasets.

Logistic Regression: For binary classification with interpretable results.

Support Vector Machine (SVM): To handle high-dimensional text data.

Random Forest: For robust ensemble learning.

Deep Learning Models: Explored using Recurrent Neural Networks (RNNs) and Transformers for more complex text understanding.

4. Evaluation Metrics

To ensure model effectiveness, the following metrics were used:

Accuracy: Overall performance of the model.

Precision: How many messages classified as spam are actually spam.

Recall (Sensitivity): How many spam messages were correctly identified.

F1 Score: A balance between precision and recall.

5. Results

The best-performing model achieved:

Accuracy: 0.9632286995515695

Precision: 0.9291338582677166

Recall: 0.7866666666666666

F1-Score: 0.851985559566787

6. Deployment

The trained model was integrated into a real-time SMS filtering pipeline:

API Deployment: The model is exposed via a RESTful API using Flask or FastAPI.
Frontend Integration: A simple user interface to classify SMS messages interactively.
