# Clickbait-Headline-Classification-Using-NLP-and-Machine-Learning
NLP-based clickbait headline detection using TF-IDF, Logistic Regression, and Linear SVM, with an interactive Gradio application.
## Project Overview

Clickbait headlines are designed to attract attention and encourage users to click on a link, often using curiosity, sensational language, emotional wording, or incomplete information.

This project develops a binary text classification system that predicts whether a given headline is:

- Clickbait
- Not Clickbait

The project demonstrates an end-to-end Natural Language Processing (NLP) and machine learning workflow.

## Key Features

- Text data loading and exploration
- Dataset cleaning
- Tokenization
- Lowercase conversion
- Stop-word removal
- Lemmatization
- Part-of-speech (POS) tagging
- Syntactic chunking
- Named Entity Recognition (NER) experimentation
- TF-IDF feature extraction
- Machine learning classification
- Model evaluation
- Interactive Gradio application

## Dataset

The project uses:

`clickbait_data.csv`

The dataset contains:

- 32,000 headlines
- 2 columns
- `headline` – headline text
- `clickbait` – binary target label

Label distribution:

| Label | Meaning | Samples |
|---|---|---:|
| 0 | Not Clickbait | 16,001 |
| 1 | Clickbait | 15,999 |

The dataset is approximately balanced.

## NLP Preprocessing

The project performs several NLP preprocessing operations, including:

1. Sentence tokenization
2. Word tokenization
3. Lowercase conversion
4. Stop-word removal
5. Lemmatization
6. POS tagging
7. Syntactic chunking
8. Named Entity Recognition experimentation

The final modeling workflow uses cleaned/lemmatized headline text.

## Machine Learning Models

The notebook evaluates text classification using:

- Logistic Regression
- Linear Support Vector Machine (Linear SVM)

TF-IDF (Term Frequency-Inverse Document Frequency) is used to convert headline text into numerical feature vectors.

## Machine Learning Pipeline

```text
Raw Headlines
      ↓
Data Cleaning
      ↓
Text Tokenization
      ↓
Lowercase Conversion
      ↓
Stop-Word Removal
      ↓
Lemmatization
      ↓
TF-IDF Vectorization
      ↓
Train/Test Split
      ↓
Machine Learning Models
      ├── Logistic Regression
      └── Linear SVM
      ↓
Model Evaluation
      ↓
Clickbait / Not Clickbait
