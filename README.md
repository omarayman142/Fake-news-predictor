# Fake-news-predictor
🧠 Text Classification using N-Gram Features:

Dataset link: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset.



📌 Overview

This project focuses on building a high-performance Text Classification model using traditional Machine Learning techniques with advanced feature engineering.

The best performance was achieved using TF-IDF with N-gram range (2,3), reaching an impressive:

🎯 98% Accuracy

🚀 Project Pipeline
1️⃣ Data Preprocessing

Text cleaning (removing punctuation, special characters)

Lowercasing

Tokenization

Removing stopwords (if applied)

2️⃣ Feature Engineering

We experimented with different N-gram ranges:

N-gram Range	Description
(1,1)	Unigrams
(1,2)	Unigrams + Bigrams
(2,2)	Bigrams only
(2,3)	Bigrams + Trigrams (Best Performance)

Best result achieved using:

TfidfVectorizer(ngram_range=(2,3))

3️⃣ Model Training

We trained multiple Machine Learning models including:

Logistic Regression

Naive Bayes

Support Vector Machine (if used)

The model trained with TF-IDF (2,3) outperformed other configurations.

📊 Results
Configuration	Accuracy
Unigram	XX%
(1,2)	XX%
(2,2)	XX%
(2,3)	98% ✅

✔️ Higher-order n-grams helped capture contextual relationships between words
✔️ Reduced ambiguity compared to single-word features

🧪 Why N-gram (2,3) Performed Better?

Captures short contextual phrases instead of isolated words

Improves semantic representation

Reduces noise from single-word tokens

Especially effective in sentiment / intent-based tasks

🛠 Tech Stack

Python

Scikit-learn

TF-IDF Vectorization

Pandas

NumPy

📂 How to Run
git clone <your-repo-link>
cd <repo-name>
pip install -r requirements.txt


Then run the notebook or training script.

📈 Future Improvements

Hyperparameter tuning

Cross-validation

Deep Learning comparison (LSTM / BERT)

Model deployment using Flask or FastAPI

👨‍💻 Author

Omar Ayman Abdelaziz
AI & Machine Learning Engineer
Interested in NLP, Computer Vision & Embedded Systems
