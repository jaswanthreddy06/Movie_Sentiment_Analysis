# 🎬 Movie Review Sentiment Analysis using NLP

A Natural Language Processing (NLP) project that classifies IMDB movie reviews as **Positive** or **Negative** using text preprocessing and machine learning models.

---

## 📌 Project Title
**Movie Review Sentiment Analysis using NLP**

## 📝 Description
This project builds a complete NLP pipeline to analyze and classify 50,000 IMDB movie reviews. It applies text cleaning, TF-IDF vectorization, and trains three ML models — Logistic Regression, Naive Bayes, and SVM — to predict the sentiment of a given review. A WordCloud visualization is also generated to highlight the most frequent words in positive and negative reviews.

---

## 📁 Project Structure

```
Movie_Sentiment_Analysis/
├── Movie_Sentiment_Analysis.ipynb    # Main Jupyter Notebook
├── IMDB Dataset.csv                  # Dataset (download from Kaggle)
└── README.md                         # Project documentation
```

---

## 🗂️ Dataset

- **Name:** IMDB Dataset of 50K Movie Reviews
- **Source:** [Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
- **Size:** 50,000 reviews (25,000 positive + 25,000 negative)
- **Columns:**
  - `review` — Raw movie review text
  - `sentiment` — Label: `positive` or `negative`

### How to Download the Dataset
1. Visit: https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews
2. Click **Download**
3. Extract the zip file
4. Place **`IMDB Dataset.csv`** in the **same folder** as the notebook

> **No internet / Kaggle account?** No worries — the notebook auto-generates a synthetic demo dataset if the CSV file is not found.

---

## ⚙️ Prerequisites

- **Python 3.8+**
- **Jupyter Notebook** or **VS Code** (with Jupyter extension)

### Install Required Libraries

The notebook includes a built-in auto-installer (Step 0). Or install manually:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk textblob wordcloud
```

---

## 🚀 How to Run

### Step 1: Clone the Repository
```bash
git clone https://github.com/jaswanthreddy06/Movie_Sentiment_Analysis.git
cd Movie_Sentiment_Analysis
```

### Step 2: Add the Dataset
Download `IMDB Dataset.csv` from Kaggle and place it in the project folder.

### Step 3: Launch Jupyter Notebook
```bash
jupyter notebook
```

### Step 4: Open the Notebook
Click on `Movie_Sentiment_Analysis.ipynb` in the Jupyter interface.

### Step 5: Run All Cells
```
Kernel → Restart & Run All
```
Or press **Shift + Enter** to run cells one by one.

> Always run **Step 0** first to install all dependencies.

---

## 🧠 Pipeline Steps

| Step | Description |
|------|-------------|
| **Step 0** | Install required libraries |
| **Step 1** | Import libraries & download NLTK data |
| **Step 2** | Load IMDB dataset (or generate synthetic data) |
| **Step 3** | Exploratory Data Analysis — distribution, review lengths |
| **Step 4** | Text cleaning — lowercase, remove HTML, stopwords, lemmatization |
| **Step 5** | TF-IDF vectorization (unigrams + bigrams, top 10,000 features) |
| **Step 6** | Train 3 ML models |
| **Step 7** | Model comparison, classification report, confusion matrix |
| **Step 8** | WordCloud for positive and negative reviews |
| **Step 9** | Predict sentiment on custom new reviews |

---

## 🤖 ML Models Used

| Model | Notes |
|-------|-------|
| **Logistic Regression** | Strong baseline; handles high-dimensional TF-IDF well |
| **Naive Bayes** | Fast and effective for text classification |
| **Support Vector Machine (SVM)** | Excellent for large-margin text classification |

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| **Language** | Python 3.x |
| **Environment** | Jupyter Notebook / VS Code |
| **Data Handling** | Pandas, NumPy |
| **NLP** | NLTK, TextBlob, Regex (re) |
| **ML Models** | Scikit-learn |
| **Vectorization** | TF-IDF (unigrams + bigrams) |
| **Visualization** | Matplotlib, Seaborn, WordCloud |
| **Version Control** | Git & GitHub |

---

## 📈 Key Findings

- **Logistic Regression** and **SVM** achieved 88–90%+ accuracy on the IMDB dataset.
- **TF-IDF with bigrams** captures two-word context (e.g., *not good*, *very bad*) for better accuracy.
- **Stopword removal** and **lemmatization** significantly reduce noise.
- WordCloud analysis shows positive reviews frequently contain: *great, love, best, wonderful, brilliant*.
- Negative reviews frequently contain: *bad, worst, boring, waste, awful, terrible*.

---
