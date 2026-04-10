# Spam Detection Model

A machine learning project to classify emails as spam or ham (non-spam) using TF-IDF vectorization and Logistic Regression.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Model Architecture](#model-architecture)
- [Installation](#installation)
- [Usage](#usage)

## Overview

This project builds a spam email detection system that can automatically classify incoming emails as either **spam** or **ham** (legitimate email). The model uses natural language processing techniques and machine learning to analyze email content and predict the category.

## Dataset

The project uses `mail_data.csv` which contains:
- **Message**: The email content/text
- **Category**: The label (spam or ham)

The dataset is split into:
- **Training Set**: 80% of the data
- **Testing Set**: 20% of the data

## Features

- **Text Preprocessing**: Handles null values and cleans email text
- **Feature Extraction**: Uses TF-IDF (Term Frequency-Inverse Document Frequency) vectorization
  - Counts word frequencies
  - Gives importance to significant words
  - Reduces importance of common words
- **Classification**: Implements Logistic Regression for binary classification
- **Model Evaluation**: Calculates accuracy metrics on training and testing data

## Model Architecture

1. **Data Loading & Preprocessing**
   - Load email data from CSV
   - Handle missing values
   - Convert labels (spam → 0, ham → 1)

2. **Feature Extraction**
   - Apply TF-IDF vectorization
   - Parameters: `min_df=1`, `stop_words='english'`, `lowercase=True`
   - Transforms raw text into numerical features

3. **Model Training**
   - Algorithm: Logistic Regression
   - Trained on 80% of the dataset

4. **Evaluation**
   - Accuracy score on training data
   - Accuracy score on testing data

## Installation

### Requirements
- Python 3.x
- numpy
- pandas
- scikit-learn

### Setup
```bash
pip install numpy pandas scikit-learn
```

## Usage

Run the Jupyter notebook `spam.ipynb` to:
1. Load and explore the email dataset
2. Preprocess the data
3. Extract features using TF-IDF
4. Train the Logistic Regression model
5. Evaluate model performance on training and testing datasets

```bash
jupyter notebook spam.ipynb
```

## Example Output

The notebook will display:
- Dataset shape and information
- Training and testing data splits
- Sample processed features
- Model accuracy on both training and testing data

