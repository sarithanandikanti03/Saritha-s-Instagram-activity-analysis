# Saritha-s-Instagram-activity-analysis
This project analyzes personal Instagram interaction data to uncover engagement patterns and evaluate machine learning models for predicting peak engagement periods. The analysis combines exploratory data analysis (EDA) with supervised learning to understand when and how user interactions are most likely to occur.

📌 Project Overview

This project analyzes personal Instagram interaction data to identify engagement patterns and build machine learning models that predict peak engagement periods. It combines exploratory data analysis (EDA) with supervised learning to compare multiple models under class imbalance conditions.

The dataset is derived from Instagram “liked posts” exported in JSON format and processed using Python.

🔍 Objectives

Understand temporal engagement behavior

Identify peak interaction hours

Analyze account-level interaction concentration

Compare multiple machine learning models fairly

Handle class imbalance using appropriate evaluation metrics

📂 Dataset

Source: Instagram liked posts (JSON export)

Format: Semi-structured JSON → pandas DataFrame

Key attributes:

Timestamp

Account name

Interaction frequency

⚠️ This dataset represents personal usage and is anonymized.

📈 Exploratory Data Analysis

The EDA focuses on:

Top accounts with the highest interactions

Engagement distribution by hour and day of week

Monthly engagement trends

Concentration analysis across accounts

Key findings:

Engagement peaks during early afternoon hours

Interaction behavior follows a clear diurnal pattern

Engagement is diversified across many accounts rather than concentrated

🤖 Predictive Modeling

To ensure a fair comparison, all models were trained on the same features and train–test split.

Models Evaluated

Logistic Regression

Random Forest Classifier

Gradient Boosting Classifier

Evaluation Strategy

Accuracy alone was avoided due to class imbalance

Used:

Precision

Recall

F1-score

Precision–Recall curves

Gradient Boosting showed better balance and was further optimized using threshold tuning

🛠️ Feature Engineering

Hour of interaction

Day of week (numeric)

Month of interaction

Account interaction frequency

Binary peak engagement label

🧪 Technologies Used

Python

pandas, NumPy

matplotlib

scikit-learn

Jupyter Notebook

⚠️ Limitations

Based on a single user’s data

Only “likes” are considered as engagement

Does not account for content quality or external trends

🚀 Future Improvements

Include comments, saves, and shares

Apply cross-validation and hyperparameter tuning

Explore time-series or sequence models

Extend analysis to multi-user datasets

▶️ How to Run
git clone <repository-url>
cd instagram-engagement-analysis
jupyter notebook

Open the notebook and run cells sequentially.

📬 Contact

For questions or feedback, feel free to reach out or open an issue
