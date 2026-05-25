# News Topic Classifier using BERT

## Project Overview
This project is a **News Topic Classification system** built using **BERT (Bidirectional Encoder Representations from Transformers)**.

The model classifies news articles into different categories using Natural Language Processing (NLP) and Deep Learning.

This task was implemented using the **AG News Dataset** and fine-tuned with Hugging Face Transformers.

---

## Objective
The main objective of this project is to classify news articles into predefined categories based on their textual content.

The model predicts the topic of a given news article.

---

## Dataset Used
**AG News Dataset**

The dataset contains news articles divided into 4 categories:

- World
- Sports
- Business
- Sci/Tech

### Dataset Files
- `train.csv`
- `test.csv`

---

## Technologies Used

- Python
- Pandas
- PyTorch
- Hugging Face Transformers
- BERT
- Scikit-learn
- Jupyter Notebook

---

## Project Workflow

### 1. Import Libraries
Imported required libraries for data handling, preprocessing, model training, and evaluation.

```python
import pandas as pd
import torch
from transformers import BertTokenizer, BertForSequenceClassification
from transformers import Trainer, TrainingArguments
```

---

### 2. Load Dataset
Loaded the training and testing datasets.

```python
train_df = pd.read_csv("train.csv")
test_df = pd.read_csv("test.csv")
```

---

### 3. Data Cleaning
Removed incorrect header rows and converted labels into integer format.

```python
train_df = train_df.iloc[1:]
test_df = test_df.iloc[1:]

train_df["label"] = train_df["label"].astype(int) - 1
test_df["label"] = test_df["label"].astype(int) - 1
```

---

### 4. Tokenization
Used BERT tokenizer to convert text into numerical tokens.

```python
tokenizer = BertTokenizer.from_pretrained("bert-base-uncased")
```

---

### 5. Model Loading
Loaded pre-trained BERT model for sequence classification.

```python
model = BertForSequenceClassification.from_pretrained(
    "bert-base-uncased",
    num_labels=4
)
```

---

### 6. Training Configuration
Configured model training parameters.

```python
training_args = TrainingArguments(
    output_dir="./results",
    num_train_epochs=1,
    per_device_train_batch_size=8,
    per_device_eval_batch_size=8
)
```

---

### 7. Model Training
Trained the model on the AG News dataset.

```python
trainer.train()
```

---

### 8. Evaluation
Evaluated the trained model on test data.

---

## Performance Optimization
To reduce training time:

- Reduced dataset size
- Used fewer epochs
- Adjusted batch size

Example:

```python
train_dataset = train_dataset.select(range(1000))
test_dataset = test_dataset.select(range(200))
```

---

## Output
The model predicts the topic of unseen news articles.

Example output:

**Input:**
Apple launches new AI-powered iPhone features.

**Predicted Topic:**
Sci/Tech

---

## Challenges Faced
During implementation, the following issues were encountered:

- Dataset header row issue
- Label conversion error
- Slow training on CPU
- Large dataset processing time

These were solved through preprocessing and dataset size reduction.

---

## Learning Outcomes
Through this task, I learned:

- Fine-tuning BERT
- Text preprocessing
- Tokenization
- Transformer-based classification
- Model training and evaluation
- Handling NLP datasets

---

## Repository Structure

```bash
news-topic-classifier/
│
├── train.csv
├── test.csv
├── news_classifier.ipynb
├── README.md
```

---

## Future Improvements

- Train on full dataset
- Improve accuracy
- Deploy as web app
- Add real-time prediction interface

---


# Additional Tasks

---

## Task 2: Customer Churn Prediction Pipeline

### Objective
Built an end-to-end machine learning pipeline to predict customer churn using Scikit-learn Pipeline API.

### What I Implemented
- Data preprocessing using Pipeline
- Feature scaling and encoding
- Logistic Regression & Random Forest models
- Hyperparameter tuning using GridSearchCV
- Model evaluation
- Exported trained pipeline using joblib

### Skills Gained
- ML pipeline construction
- Hyperparameter tuning
- Model optimization
- Pipeline deployment readiness

### Tools Used
- Python
- Scikit-learn
- Pandas
- Joblib

---

## Task 3: Auto Tagging Support Tickets Using LLM

### Objective
Built an automated support ticket tagging system using Large Language Models (LLMs).

### Dataset
Free-text Support Customer Ticket Dataset

### What I Implemented
- Zero-shot classification
- Few-shot prompt engineering
- Compared zero-shot vs few-shot performance
- Generated top 3 probable tags for each ticket
- Multi-class text classification

### Skills Gained
- Prompt engineering
- LLM-based classification
- Zero-shot & few-shot learning
- Ranking predictions

### Tools Used
- Python
- Transformers
- Hugging Face
- LLM Prompt Engineering

## Author
Developed as part of an NLP / Machine Learning learning project.
