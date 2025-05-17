<<<<<<< HEAD
<<<<<<< HEAD
# 📘 Twitter Entity Sentiment Analysis

This project performs **entity-based sentiment analysis** on tweets using a publicly available dataset from Kaggle. The aim is to identify named entities (like organizations, people, products) and determine the **sentiment** expressed about them within each tweet.

## 📂 Dataset

- **Source:** [Kaggle - Twitter Entity Sentiment Analysis](https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis)
- The dataset contains tweets annotated with:
  - `entity`: Entity mentioned in the tweet.
  - `sentiment`: Sentiment expressed about the entity (`positive`, `neutral`, `negative`).
  - `content`: Raw tweet text.

## 📊 Project Objectives

- Preprocess and clean tweet text.
- Visualize sentiment and entity distribution.
- Extract features using TF-IDF.
- Train a machine learning model (SVC) to classify sentiment.
- Evaluate the model's performance.

## 🚀 Technologies Used

- **Python** 🐍
- **Jupyter Notebook** 📓
- **Libraries**:
  - `pandas`, `numpy` for data handling
  - `matplotlib`, `seaborn` for visualizations
  - `nltk`, `re` for NLP and text cleaning
  - `scikit-learn` for modeling and evaluation

## 🧹 Data Preprocessing

Each tweet undergoes the following preprocessing steps:

- Convert text to lowercase.
- **Remove**:
  - Emojis
  - Hashtags (`#example`)
  - Mentions (`@user`)
  - URLs (`http://...`, `https://...`)
  - Numbers
  - HTML/XML tags (e.g., `<div>`)
  - Punctuation and extra whitespace
- **Replace**:
  - Slang and abbreviations (e.g., `AFK` → "away from keyboard", `GG` → "good game") using a custom slang dictionary.
- **Text normalization**:
  - Tokenization
  - Stopword removal (using NLTK)
  - Lemmatization

## 📈 Visualizations

- Sentiment distribution bar chart
- Word clouds for each sentiment
- Top entities by frequency

## 🧠 Feature Extraction

- Use **TF-IDF Vectorization** to convert cleaned tweet text into numerical feature vectors for model input.

## 🔍 Model Training

- Model used: **Support Vector Classifier (SVC)**
- Train on TF-IDF features to predict sentiment labels (`positive`, `neutral`, `negative`)
- Evaluate using:
  - Accuracy
  - Confusion Matrix
  - Classification Report (precision, recall, F1-score)

## 📁 Repository Structure

```
Twitter_Sentiment_Analysis/
├── twitter_Analysis.ipynb # Main notebook for EDA, preprocessing, and modeling
├── data/
│   └── Twitter/
|           └── twitter_training.csv
|           └── twitter_validation.csv
├── README.md # Project overview file
└── main.py # Python dependencies
```
=======

>>>>>>> bc5b46a0bfe673c9d0b98bfc67065b03c0ea23d8
