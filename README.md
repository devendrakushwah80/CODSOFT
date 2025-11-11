# 💳 Credit Card Fraud Detection  
### 🚀 A Machine Learning Journey by *Devendra Kushwah*

---

## 📘 Project Overview
Every year, millions of people lose money because of fraudulent credit card transactions.  
So I decided to build a **Fraud Detection System** that can automatically spot suspicious transactions  
— using **Machine Learning** and a bit of smart data balancing 🧠.

The dataset used is from **Kaggle (Kartik Shenoy’s Credit Card Fraud Dataset)**.  
It contains thousands of transactions labeled as either **fraudulent (1)** or **legitimate (0)**.

---

## 🧩 My Thought Process (Story Mode 🎬)

When I started this project, I honestly thought it was going to be simple —  
train a model, get accuracy, done. But as soon as I saw my first results, I got **99% accuracy** 😳

At first, I was like:
> “Wait... did I just build a super accurate fraud detector or is my model cheating?”

That’s when the **real detective work** began 🕵️‍♂️  

I checked:
- Is my dataset balanced? (Nope, it was heavily skewed!)
- Am I overfitting? (Maybe…?)
- Are my results real or just because most data is non-fraud?

So, I dug deeper 🔍  
I used **SMOTE** to balance the data,  
applied **Standard Scaling**, and then trained a **Random Forest Classifier**  
with `class_weight='balanced'` to make sure the model pays attention to both classes equally.

Then came the “Oh yes!” moment 🎉  
After checking **Train vs Test Accuracy**, I found:

| Metric | Score |
|---------|--------|
| Train Accuracy | 99.59% |
| Test Accuracy | 99.46% |

The difference was tiny — meaning **no overfitting!**  
My model actually learned the patterns instead of memorizing the data 💪

---

## 🧠 Key Features
- Preprocessing: Cleaned and encoded categorical variables  
- Feature Engineering: Extracted hour, day, month, weekday from transaction time  
- Balancing: Used **SMOTE** to handle imbalanced classes  
- Model: **Random Forest Classifier** with tuned hyperparameters  
- Evaluation: Accuracy, Confusion Matrix, Precision-Recall, ROC-AUC  
- Model Saving: Exported model using `joblib` for future predictions  

---

## 📊 Evaluation Metrics

| Metric | Score |
|--------|--------|
| Accuracy | **99.45%** |
| ROC-AUC | **0.99+** |
| Precision (Fraud Class) | High ✅ |
| Recall (Fraud Class) | High ✅ |

📈 **Confusion Matrix Visualization:**
Shows how well the model differentiates between Fraud and Non-Fraud transactions.

---

## 🧮 Libraries Used
```python
pandas, numpy, matplotlib, seaborn  
scikit-learn, imblearn (SMOTE), joblib
