# SMS-spm_detection
SMS spm detection using machine learning
# 📩 SMS Spam Detection using NLP & Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-blue.svg?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/scikit--learn-ML-orange.svg?logo=scikit-learn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/NLP-TF--IDF-yellow.svg" alt="NLP">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/Made%20with-Jupyter-orange.svg?logo=jupyter&logoColor=white" alt="Jupyter">
</p>

<p align="center">
  A Natural Language Processing project that classifies SMS messages as <b>Spam</b> or <b>Ham</b>, using TF-IDF vectorization with Naive Bayes and Logistic Regression — complete with EDA, confusion matrices, and live testing on custom messages.
</p>

<p align="center">
  <a href="https://colab.research.google.com/github/YOUR-USERNAME/YOUR-REPO/blob/main/SMS_Spam_Detection.ipynb">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab">
  </a>
</p>

---

## 📌 Overview

This project builds a text classifier that detects spam SMS messages using classic NLP techniques. It walks through the full pipeline — cleaning raw text, converting it into numerical features with TF-IDF, training two different models, and evaluating which performs better.

## ✨ Features

- 📊 Exploratory Data Analysis — class balance and message length distributions
- 🧹 Text preprocessing (lowercasing, punctuation removal, whitespace cleanup)
- 🔢 Feature extraction using **TF-IDF** vectorization
- 🤖 Two trained models: **Multinomial Naive Bayes** and **Logistic Regression**
- 📈 Evaluation via accuracy, classification report, and confusion matrices
- 🧪 Live testing — try your own custom messages and see instant predictions
- ☁️ Runs entirely in Google Colab — no downloads or setup required

## 🖼️ Preview

| Class Distribution | Message Length by Label | Confusion Matrices |
|:---:|:---:|:---:|
| Spam vs Ham count plot | Histogram comparing lengths | Side-by-side model comparison |

*(Generated automatically when you run the notebook — screenshots can be added here after your first run.)*

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3 |
| Data Handling | pandas, NumPy |
| Visualization | matplotlib, seaborn |
| NLP / ML | scikit-learn (TF-IDF, Naive Bayes, Logistic Regression) |
| Environment | Google Colab / Jupyter Notebook |

## 📁 Project Structure

```
sms-spam-detection/
├── SMS_Spam_Detection.ipynb   # Main notebook (EDA + NLP pipeline + models)
└── README.md                  # Project documentation
```

## 🚀 Getting Started

### Run in Google Colab (recommended)
1. Click the **"Open in Colab"** badge above
2. Go to `Runtime → Run all`
3. The dataset loads automatically from a public URL — no downloads needed

### Run locally
```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook SMS_Spam_Detection.ipynb
```

## 🧠 Methodology

1. **Load Data** — SMS Spam Collection dataset (public dataset, loaded via URL)
2. **Explore** — visualize spam vs ham distribution and message length patterns
3. **Clean Text** — lowercase, strip punctuation/numbers, normalize whitespace
4. **Vectorize** — convert text into numerical features using TF-IDF
5. **Train Models** — Multinomial Naive Bayes and Logistic Regression
6. **Evaluate** — accuracy, precision/recall, confusion matrix comparison
7. **Test** — run predictions on custom, unseen messages

## 📊 Results

| Model | Accuracy ↑ |
|---|:---:|
| Multinomial Naive Bayes | ~95% |
| **Logistic Regression** | **~96%+** |

> Both models perform strongly on this dataset, with Logistic Regression slightly ahead. *(Exact values may vary slightly by run/library version.)*

**Sample predictions:**
```
"Congratulations! You've won a free iPhone. Click here to claim now!" → SPAM
"Hey, are we still meeting for lunch tomorrow?"                       → HAM
```

## 🗺️ Roadmap

- [ ] Try transformer-based models (e.g., BERT via Hugging Face)
- [ ] Handle class imbalance explicitly (SMOTE, class weighting)
- [ ] Add n-gram features to TF-IDF for richer context
- [ ] Deploy as a real-time message classifier (Streamlit/Flask app)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m "Add YourFeature"`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

