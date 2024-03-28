# Chatbot Model with Doc2Vec for School Dataset

## Introduction

This repository contains code for training a chatbot model specialized for school-related questions and answers using a Doc2Vec model. The model is trained on a dataset in English.

## Prerequisites

Ensure you have the following libraries installed in your Python environment:
- pandas
- nltk
- gensim
- scikit-learn
- langdetect

## Dataset

The dataset used for training is stored in an Excel file named `Dataset_EFREI_en.xlsx`. It contains two columns: "Question" and "Answer" scrapped from my school official website.

## Pre-processing

Pre-processing steps applied to the dataset:
- Convert text to lowercase
- Remove URLs, mentions, hashtags, and emojis
- Remove punctuation
- Tokenize text
- Remove stop words
- Lemmatization and stemming

## Training

The Doc2Vec model is trained using the pre-processed dataset. Similar questions are retrieved for every question in the dataset for testing. 
The similarity between questions is calculated using the trained Doc2Vec model.

## Testing
The chatbot's performance is evaluated by testing it on a subset of questions from the dataset. For each question, the model retrieves the most similar questions along with their corresponding answers. If the similarity score is below 50%, a message is sent to the user indicating that the question cannot be answered accurately. The results are printed for analysis.

## Conclusion
The model demonstrates good performance when answering questions from the dataset. It also handles questions outside the dataset well, especially those containing key words present in the training data. However, when encountering questions with no relevant information in the dataset, or when similarity scores are below 50%, the model's performance may be less accurate, prompting a notification to the user.
