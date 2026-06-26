# 💬 Customer Sentiment Analysis — NLP Text Mining Pipeline

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-NLTK%20%7C%20TF--IDF-blue?style=flat-square)
![TextBlob](https://img.shields.io/badge/TextBlob-Sentiment%20Analysis-green?style=flat-square)
![Accuracy](https://img.shields.io/badge/Accuracy-88%25-brightgreen?style=flat-square)

> End-to-end NLP pipeline classifying customer reviews into Positive, Negative, and Neutral sentiment using TF-IDF vectorization and NLTK — achieving 88% classification accuracy.

---

## 📌 Problem Statement
Businesses receive thousands of unstructured customer reviews daily. Manually reading them is impossible at scale. This project automates sentiment classification to surface actionable product and service improvement insights from raw review text.

## 🎯 Results

| Metric | Score |
|--------|-------|
| **Accuracy** | **88%** |
| Precision (Weighted) | 87% |
| Recall (Weighted) | 88% |
| F1-Score (Weighted) | 87% |
| Vectorization | TF-IDF |
| Classifier | Logistic Regression + NLTK preprocessing |
| Task | Multiclass Sentiment Classification |

## 🛠️ Tech Stack
- **Language:** Python
- **NLP:** NLTK, TextBlob, TF-IDF (Scikit-learn)
- **ML:** Logistic Regression, Scikit-learn
- **Data Processing:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, WordCloud
- **Environment:** Jupyter Notebook

## 📂 Project Structure
```
nlp-reviews-text-mining/
├── data/          # Customer reviews dataset
├── python/        # Notebooks & scripts
├── requirements.txt
└── README.md
```

## 🚀 How to Run
```bash
git clone https://github.com/shreesneha056-gif/nlp-reviews-text-mining.git
cd nlp-reviews-text-mining
pip install -r requirements.txt
jupyter notebook
```

## 📊 Pipeline Overview
1. **Data Loading** — Load and explore customer review dataset
2. **Text Preprocessing** — Tokenization, stopword removal, lemmatization (NLTK)
3. **Feature Extraction** — TF-IDF vectorization
4. **Sentiment Classification** — Positive / Negative / Neutral (88% accuracy)
5. **Exploratory Text Analysis** — Word frequencies, N-grams, word clouds
6. **Business Insights** — Actionable product improvement recommendations

---
📫 [LinkedIn](https://www.linkedin.com/in/sneha-shree-mu/) | [Portfolio](https://shreesneha056-gif.github.io/portfolio_website/) | [GitHub](https://github.com/shreesneha056-gif)
