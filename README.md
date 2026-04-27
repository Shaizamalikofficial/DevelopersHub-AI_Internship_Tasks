# DeveloperHub-AI_Internship_Tasks
## – Data Analysis & Machine Learning -

This repository contains three tasks completed as part of my AI Internship. Each task focuses on different aspects of Data Analysis, Visualization and Machine Learning Modeling.

---

# 🔹 Task 1: Exploring and Visualizing a Dataset

## 📌 Objective

To understand the dataset by performing Data Inspection, StatisticalAanalysis and Visualization.

## 📂 Dataset Used

* Iris Dataset (loaded using seaborn)

## ⚙️ Work Performed

* Loaded dataset using pandas
* Explored dataset structure using `.shape`, `.head()`, `.info()`, `.describe()`
* Analyzed feature distributions and relationships
* Created visualizations:

  * Scatter plots
  * Histograms
  * Box plots
  * Pairplot

## 📈 Key Findings

* Dataset was clean with no missing values
* Petal features showed better separation between species
* Setosa species was clearly distinguishable while others had slight overlap
* Visualizations helped identify patterns and relationships effectively

---

# 🔹 Task 2: Stock Price Prediction (Short-Term)

## 📌 Objective

To Predict the Next Day’s Closing Stock Price using Historical Data.

## 📂 Dataset Used

* Stock market data fetched using `yfinance` (Apple stock)

## ⚙️ Work Performed

* Retrieved historical stock data
* Created target variable (`Next_Close`) using shifting technique
* Selected features: Open, High, Low, Volume
* Applied time-based train-test split
* Trained **Random Forest Regressor**
* Generated predictions and visualized results

##  Evaluation Metrics

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* R² Score

## 📈 Key Findings

* Model successfully captured overall price trends
* Predictions were close to actual values with slight deviations
* Random Forest performed well due to handling non-linear patterns
* Stock price volatility limits perfect prediction accuracy

---

# 🔹 Task 3: House Price Prediction

## 📌 Objective

To Predict House Prices based on Property Features such as Size, Location and Condition.

## 📂 Dataset Used

* House Price Prediction Dataset (Kaggle)

## ⚙️ Work Performed

* Cleaned dataset and handled missing values
* Dropped irrelevant features (street, country)
* Converted date into year and month
* Encoded categorical variables (city, statezip)
* Applied feature scaling
* Trained **Gradient Boosting Regressor**
* Generated predictions and visualized results

## Evaluation Metrics

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

## Key Findings

* Features like Living Area, Location and Condition strongly influenced prices
* Model predictions aligned well with actual values
* RMSE highlighted larger prediction errors effectively
* Model captured complex relationships between features and price

---

# 🔹 Overall Learning

Through these tasks, I gained hands-on experience in:

* Data Preprocessing and Feature Engineering
* Exploratory Data Analysis (EDA)
* Regression Modeling Techniques
* Model Evaluation using appropriate metrics
* Data Visualization for better insights

---

# Author (Shaiza Malik)

AI Intern – Data Science & Machine Learning  
This repository contains my hands-on implementation of AI/ML concepts learned during the internship including Data Analysis, Visualization and Predictive Modeling.

