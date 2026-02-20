# Multi-Class Movie Review Sentiment Classification

This project focuses on building a multi-class classification model to predict the sentiment of movie reviews.

The model is evaluated using **accuracy** as the primary metric.

## Problem Statement

A movie review platform wants to analyze user sentiments from posted reviews.  
Each review is categorized into one of three sentiment classes:

- 0 → Negative  
- 1 → Neutral  
- 2 → Positive  

The dataset includes the original review text (`phrase`) along with three engineered numerical features.

---

## Dataset Description

### Features

- `id` – Unique identifier  
- `phrase` – Movie review text  
- `feature_1` – Engineered feature  
- `feature_2` – Engineered feature  
- `feature_3` – Engineered feature  
- `sentiment` – Target label

---

## Approach

### 1. Exploratory Data Analysis
- Checked class distribution
- Analyzed review length patterns
- Inspected correlation between engineered features

### 2. Text Preprocessing
- Lowercasing
- Removal of punctuation and special characters
- Tokenization
- Stopword removal

### 3. Feature Engineering
- TF-IDF vectorization of review text
- Combined text vectors with structured numerical features
- Feature scaling where required

### 4. Model Training
- Benchmarked multiple classifiers such as:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
  - Support Vector Machines
- Used cross-validation for model comparison
- Performed hyperparameter tuning on the top model

### 5. Evaluation Metric
- Accuracy

---

## Results

- Achieved strong classification accuracy on validation data.
- Selected the best-performing model based on cross-validation accuracy.
- Generated predictions for the test set for submission.

---

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn

---
