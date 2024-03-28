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

## Training and Testing

The Doc2Vec model is trained using the pre-processed dataset. Similar questions are retrieved for every question in the dataset for testing. 
The similarity between questions is calculated using the trained Doc2Vec model.
