# 🔍 Duplicate Question Detector

## Overview

A machine learning-powered web application that determines whether two questions are duplicates or semantically similar.

Have you ever searched for an answer online and wondered whether someone has already asked the same question? This application uses Natural Language Processing (NLP) and Machine Learning techniques to analyze pairs of questions and predict whether they represent the same intent.

🚀 **Try the live application here:**  
[Duplicate Question Detector - Streamlit App](https://double-trouble-esterhazytorte.streamlit.app/)

---

## Features

- 📝 Accepts two user-provided questions
- 🤖 Predicts whether the questions are duplicates or not
- ⚡ Provides real-time predictions through an interactive web interface
- 📊 Built using a complete machine learning pipeline from preprocessing to deployment

---

## Project Workflow

The application follows an end-to-end NLP classification pipeline:

1. **Text Preprocessing**
   - Converted text to lowercase
   - Removed HTML tags and unnecessary characters
   - Removed punctuation and performed text normalization
   - Applied stopword handling and preprocessing techniques

2. **Feature Engineering**
   - Extracted text similarity features from question pairs
   - Created additional linguistic features to capture question relationships

3. **Feature Extraction**
   - Applied **Bag-of-Words (BoW)** vectorization
   - Combined sparse text representations with engineered features

4. **Model Training**
   - Trained and compared multiple machine learning algorithms:
     - Logistic Regression
     - Naive Bayes
     - Decision Tree
     - Random Forest

5. **Model Evaluation**
   - Evaluated models using:
     - Accuracy score
     - Confusion matrix analysis

6. **Deployment**
   - Deployed the final model as an interactive **Streamlit web application**

---

## Model Performance

The best-performing model was:

| Model | Accuracy |
|---|---|
| Random Forest | **78%** |
| Naive Bayes   | **72%** |
| Logistic Regression | **74%** |
| Decision Tree | **74%** |

The Random Forest classifier was selected due to its performance compared to the other evaluated models and lesser number of False Positives.

---

## Technologies Used

### Programming Language
- Python

### Machine Learning & NLP
- Scikit-learn
- Natural Language Processing (NLP)
- Bag-of-Words (BoW)
- Feature Engineering

### Data Processing
- Pandas
- NumPy
- NLTK
- BeautifulSoup

### Deployment
- Streamlit

### Model Serialization
- Pickle / Joblib

---
