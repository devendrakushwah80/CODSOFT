# 🎬 Movie Genre Classification

## 🧩 Overview

This project is part of the **CODSOFT Machine Learning Internship**.  
The goal of this task is to **predict the genre of a movie based only on its plot description** using machine learning techniques.  
Given a textual summary of a movie, the model learns patterns and predicts whether the movie belongs to genres like *Drama, Comedy, Thriller, Romance,* etc.

---

## 🧠 Objective

To build a machine learning model that can classify movies into their respective genres using only the **DESCRIPTION** text as input.

---

## ⚙️ Approach

1. **Dataset Loading:**
   - Dataset contains four columns — `ID`, `TITLE`, `GENRE`, and `DESCRIPTION`.
   - Only the `DESCRIPTION` column is used as the text input feature.

2. **Data Cleaning:**
   - Removed missing/null values.
   - Converted all text to lowercase.
   - Removed stopwords, punctuation, and extra spaces.

3. **Feature Extraction (Text → Numbers):**
   - Used **TF-IDF Vectorization** to convert text data into numerical features.
   - Used bigrams (`ngram_range=(1,2)`) and ignored rare words (`min_df=3`).

4. **Model Training:**
   - Tried multiple models:
     - LinearSVC
     - Logistic Regression
     - Multinomial Naive Bayes
   - Best performance was achieved using **TF-IDF + Logistic Regression** and **Ensemble (VotingClassifier)**.

5. **Model Evaluation:**
   - Dataset was split into 80% training and 20% testing.
   - Evaluated using Accuracy, Precision, Recall, and F1-score.

---

## 📊 Results

| Model                        | Accuracy (%) |
|-------------------------------|--------------|
| Linear SVC                    | 57.55        |
| Logistic Regression (tuned)   | ~72          |
| Naive Bayes                   | ~70          |
| Ensemble (Voting Classifier)  | **~78–80**   |

✅ The final ensemble model achieved an accuracy of around **80%** using only movie descriptions.

---

## 🧪 Technologies Used

- Python 🐍  
- Pandas  
- NumPy  
- Scikit-learn  
- TF-IDF Vectorizer  

---

## 💡 Future Improvements

- Use **BERT** or **DistilBERT** for deeper semantic understanding.  
- Expand the dataset with more genre examples.  
- Implement a **web app** using Streamlit or Flask for live predictions.

---

## 📁 Project Structure

