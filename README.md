# Fake_news_Prediction

📰 Fake News Detection using Machine Learning

This project is a machine learning-based Fake News Classifier that predicts whether a news article is Real or Fake using NLP techniques such as TF-IDF vectorization and Logistic Regression.
The app is deployed using Streamlit, allowing users to enter any news text and get instant predictions.

🚀 Features

✔ Machine Learning model (Logistic Regression) trained on Kaggle’s fake-news dataset

✔ TF-IDF Vectorizer for text feature extraction

✔ Clean and scalable Streamlit web app

✔ Real-time prediction of True or Fake news

✔ Preprocessing pipeline: stopwords removal, punctuation cleaning, tokenization

✔ Model saved using joblib for deployment

🌐 Live Demo (Streamlit Cloud)
👉 https://fakenewsprediction-2nxbvgvqhfyqdvt6q5heh3.streamlit.app/

📌 About the Project

Fake news spreads rapidly, especially through social media.
This project uses NLP + Machine Learning to classify any text news article as:

✔ Real
✖ Fake

🔧 Model Training Pipeline

The model was trained using the Jupyter Notebook app.ipynb.

Steps include:

1️⃣ Text Preprocessing

Convert to lowercase

Remove URLs

Remove punctuation

Remove numbers

Remove stopwords

Tokenization

2️⃣ Vectorization

Used TF-IDF (max_features=5000) to convert text into numerical form.

Saved as:

vectorizer.jb

3️⃣ Model Used

A Logistic Regression classifier was trained on the TF-IDF vectors.

Saved as:

lr_model.jb

🧪 Example Usage (Streamlit App)

User enters a news article text

The app transforms it using the saved vectorizer

TF-IDF features are passed to the trained model

Output:

✔ Real News
✖ Fake News

<img width="785" height="411" alt="image" src="https://github.com/user-attachments/assets/26646828-40df-4803-8b47-79cdef263f54" />



A Logistic Regression model trained on true.csv and fake.csv datasets performs the predictions.

💡 Challenges & Solutions
🔸 Problem: Model predicted True CSV correctly but new real news incorrectly

Cause: TF-IDF vocabulary mismatch and overfitting.
Fix:

Added n-grams

Improved preprocessing

Merged title + text

Cleaned input before prediction

Ensured same vectorizer is used during training and prediction




