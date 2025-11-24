# 📧 Spam vs Ham Email Classifier (Naive Bayes + TF-IDF)

This project is a **machine learning model** that classifies SMS/email messages into:
- **Ham (Not Spam)**
- **Spam**

It uses **TF-IDF Vectorization** + **Naive Bayes Classifier** for text classification.

---

## 🚀 Project Workflow
1. Load the dataset (`spam.csv`)
2. Preprocess data (labels → numbers)
3. Convert text → numbers using **TF-IDF**
4. Train **Naive Bayes Classifier**
5. Evaluate performance (Accuracy, Confusion Matrix, Classification Report)

---

## 📂 Dataset
We used the **SMS Spam Collection Dataset**:
- [Kaggle Link](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)

Place the file in `data/spam.csv`.

---

## ⚡ Results
- Accuracy: ~97-98%
- Strong performance on Spam detection
- Confusion Matrix visualization

---

## 🛠️ Requirements
Install dependencies using:
```bash
pip install -r requirements.txt
