# Machine Learning & NLP Tasks

This repository contains three machine learning and NLP projects focused on classification, pipeline development, and LLM-based automation.

---

# Task 1: News Topic Classifier using BERT

## Objective
Build a news classification model to categorize news articles into different topics using BERT.

## Methodology / Approach
- Used AG News Dataset
- Preprocessed and cleaned text data
- Applied tokenization using BERT tokenizer
- Fine-tuned BERT for sequence classification
- Trained and evaluated model using Hugging Face Trainer API

## Key Results / Observations
- Successfully classified news into 4 categories
- Achieved efficient text classification using transformer models
- Observed that reducing dataset size improved training speed

---

# Task 2:  End-to-End ML Pipeline with Scikit-learn Pipeline API

## Objective
Develop an end-to-end reusable ML pipeline to predict customer churn.

## Methodology / Approach
- Built preprocessing pipeline for scaling and encoding
- Trained Logistic Regression and Random Forest models
- Applied GridSearchCV for hyperparameter tuning
- Exported final pipeline using joblib

## Key Results / Observations
- Built a production-ready ML workflow
- Improved model performance through hyperparameter tuning
- Enabled reusable deployment pipeline

---

# Task 3: Auto Tagging Support Tickets using LLM

## Objective
Automatically classify support tickets into relevant categories using LLM.

## Methodology / Approach
- Used free-text support ticket dataset
- Applied zero-shot and few-shot prompting
- Compared prompt engineering strategies
- Generated top 3 probable tags for each ticket

## Key Results / Observations
- Few-shot prompting improved classification accuracy
- LLM handled multi-class text categorization effectively
- Generated ranked tag predictions for support automation

---

## Technologies Used
- Python
- Scikit-learn
- Hugging Face Transformers
- BERT
- Pandas
- PyTorch
- Joblib
- LLM Prompt Engineering
