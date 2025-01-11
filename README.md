# Sentiment Analysis on IMDB Dataset using LSTM

This repository contains a Python script for performing sentiment analysis on the IMDB movie review dataset using an LSTM (Long Short-Term Memory) model. The script preprocesses the text data, tokenizes it, and trains an LSTM model to classify movie reviews as either positive or negative.

## Overview

Sentiment analysis is a natural language processing (NLP) task that involves determining the sentiment expressed in a piece of text. This project uses an LSTM-based deep learning model to classify IMDB movie reviews as either positive or negative.

## Dataset
The dataset used in this project is IMDB.csv, which contains 50,000 movie reviews labeled with sentiment (positive or negative). The dataset is preprocessed to convert labels to binary values: positive → 1 and negative → 0.

## Preprocessing
The preprocessing steps include:
- Cleaning the text by removing URLs, special characters, and stopwords.
- Tokenizing the text and converting it into sequences.
- Padding the sequences to ensure uniform length.

##   Model Architecture
The model architecture consists of:
1. An Embedding layer to convert tokens into dense vectors.
2. An LSTM layer to capture sequential information.
3. A Dense layer with a sigmoid activation function for binary classification.

## Training
The model is trained using the Adam optimizer and binary cross-entropy loss. The training process runs for 5 epochs with a batch size of 32.

##Evaluation
The model's performance is evaluated using a classification report, which includes precision, recall, and F1-score.
