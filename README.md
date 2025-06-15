# 🧠 Financial News Sentiment Classification (Multiclass NLP Project)

This project builds and compares multiple machine learning models to classify financial news headlines into three sentiment categories: **Positive**, **Negative**, and **Neutral**. It uses real-world datasets and common NLP techniques to build a pipeline for sentiment modeling.

---

## 🔍 Objective

To develop a robust multiclass sentiment classifier using machine learning and NLP on financial news data, with a focus on model interpretability and class balance.

---

## 📦 Dataset

- **Financial PhraseBank Dataset**  
  Source: [Kaggle](https://www.kaggle.com/datasets/ankurzing/sentiment-analysis-for-financial-news)  
  Contains labeled financial headlines across 3 classes: Positive, Negative, Neutral.

- **Headlines Dataset**  
  Source: News Archive  
  Unlabeled financial headlines used for inference and trend analysis.

---

## 📊 Techniques Used

- **Text Preprocessing**: lowercasing, punctuation removal, regex cleaning
- **Feature Engineering**: TF-IDF Vectorization
- **Supervised Learning Models**:
  - ✅ Logistic Regression (with class weights)
  - 📉 Multinomial Naive Bayes
  - ⚡ XGBoost Classifier
- **Evaluation Metrics**:
  - Accuracy, Precision, Recall, F1-Score
  - Confusion Matrix Visualization

---

## 🧪 Model Performance Summary

| Model               | Accuracy | Macro F1 | Best At                |
|---------------------|----------|----------|-------------------------|
| Logistic Regression | 76%      | 0.72     | Best overall balance ✅ |
| XGBoost Classifier  | 76%      | 0.68     | Strong Neutral recall   |
| Naive Bayes         | 69%      | 0.48     | Overfitted to Neutral   |

Logistic Regression with `class_weight='balanced'` achieved the best class balance and is recommended for deployment.

---

## 📈 Visual Results

### 📊 Sentiment Distribution (Training Set)
![Bar Plot](outputs/charts/sentiment_distribution_barplot.png)

### 📆 Monthly Sentiment Trends (Unlabeled Data)
![Line Chart](outputs/charts/sentiment_distribution_lineplot.png)

### 🤖 Confusion Matrix – Logistic Regression
![Confusion Matrix LR](outputs/charts/confusion_matrix_lr.png)

### 🤖 Confusion Matrix – XGBoost
![Confusion Matrix XGB](outputs/charts/confusion_matrix_xgb.png)

---

## 🛠️ Tools Used

- **Languages**: Python
- **Libraries**: scikit-learn, XGBoost, Pandas, Matplotlib, Seaborn
- **ML Techniques**: TF-IDF, Logistic Regression, Naive Bayes, XGBoost
- **Visualization**: Matplotlib & Seaborn
- **Jupyter Notebooks** for exploration, modeling, and reporting

---

## 📁 Folder Overview

