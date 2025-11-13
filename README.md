# 📱 WhatsApp Review Sentiment Analysis (NLP Project)

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![NLP](https://img.shields.io/badge/Field-Natural_Language_Processing-green)

## 📌 Project Overview
This project focuses on **Sentiment Analysis** of user reviews for the WarThunder application on the Google Play Store. The goal is to classify user feedback into **Positive** or **Negative** sentiments to understand user satisfaction and identify potential app issues.

As an Electrical Automation Engineering student, I developed this project to bridge the gap between raw data collection and intelligent decision-making systems.

## ⚙️ Methodology & Workflow

### 1. Data Acquisition (`Scrap.ipynb`)
* **Source:** Google Play Store.
* **Tool:** `google-play-scraper` library.
* **Volume:** Scraped approximately 10,000 user reviews (Indonesian language).

### 2. Data Preprocessing (`Analisis_sentiment.ipynb`)
To ensure high model accuracy, the raw text underwent rigorous cleaning:
* **Casefolding:** Converting text to lowercase.
* **Cleaning:** Removing punctuation, numbers, and special characters using Regex.
* **Slang Normalization:** Converting informal Indonesian words (e.g., "yg", "ga") to formal words using a custom dictionary (`Slang_indo.txt`).
* **Stopword Removal:** Removing common non-essential words using NLTK.
* **Stemming:** Reducing words to their root form using **Sastrawi**.

### 3. Modeling
* **Feature Extraction:** TF-IDF (Term Frequency-Inverse Document Frequency).
* **Algorithm:** Support Vector Machine (SVM) / Naive Bayes
* **Evaluation:** Confusion Matrix, Accuracy, and F1-Score.

## 📂 File Structure
* `Scrap.ipynb`: Notebook for scraping data from Play Store.
* `Analisis_sentiment.ipynb`: Main notebook for preprocessing, visualization, and modeling.
* `Slang_indo.txt`: Dictionary for normalizing Indonesian slang words.
* `ulasan_aplikasi.csv`: Raw dataset.
* `requirements.txt`: List of dependencies.

## 🚀 How to Run
1.  Clone this repository.
2.  Install dependencies: `pip install -r requirements.txt`
3.  Run `Scrap.ipynb` to get fresh data (optional).
4.  Run `Analisis_sentiment.ipynb` to train and evaluate the model.

---
**Author:** Rafi Achmad Nabihan
