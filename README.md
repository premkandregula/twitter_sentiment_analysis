# twitter_sentiment_analysis
# 🐦 Twitter Sentiment Analysis

This project performs **sentiment analysis on Twitter data**, specifically to identify whether a tweet contains **racist content (label 1)** or **non-racist content (label 0)** using NLP and machine learning techniques.

---

## 📘 Overview

This is an **entity-level sentiment classification** project using a dataset of over **29,530 tweets**. The objective is to detect offensive or racist content using Logistic Regression after extensive data preprocessing.

---

## 📂 Dataset Information

- **Source**: Pre-collected CSV file (`Twitter Sentiments.csv`)
- **Columns**:
  - `id`: Tweet ID
  - `label`: 0 (not racist), 1 (racist)
  - `tweet`: Raw tweet text

---

## 🚦 Workflow Steps

### 1. 📥 Data Loading
- Read CSV using `pandas`.
- Basic info and shape inspection.

### 2. 🧹 Data Preprocessing
- Remove Twitter handles (`@user`) using regex.
- Remove special characters, digits, and punctuation.
- Remove short words (less than 3 characters).
- Tokenization.
- **Stemming** using `PorterStemmer` from NLTK.
- Combine stemmed words into cleaned tweets.

### 3. 📊 Exploratory Data Analysis (EDA)
- Generate a **word cloud** for all tweets and positive tweets.
- Frequency analysis of words.

### 4. ✂️ Train-Test Split
- Use `train_test_split` to divide the data for modeling.

### 5. 🤖 Model Building
- **Logistic Regression** is trained on the cleaned tweet data.

### 6. 🔮 Prediction
- Trained model is used to predict sentiment on new tweet data.

---

## 📦 Requirements

```bash
pip install -r requirements.txt
```

---

## 🖼️ Visualizations

- Word clouds for full dataset and per sentiment label.
- Frequency plots for most common words.

---

## 🚀 Getting Started

1. Clone this repository or download the notebook.
2. Place the dataset file `Twitter Sentiments.csv` in the specified directory.
3. Run the notebook `Twitter Sentiment Analysis.ipynb` in Jupyter Lab or Google Colab.
4. View sentiment classification results and visualizations.

---


## 📌 Future Enhancements

- Integrate deep learning models (LSTM, BERT)
- Add Streamlit web interface for live tweet classification
- Evaluate using metrics like F1-score, ROC-AUC
- Deploy model as an API

## ## 🔗 Connect with Me

[LinkedIn Profile](https://www.linkedin.com/in/kandregula-prem-kumar-059642238)

