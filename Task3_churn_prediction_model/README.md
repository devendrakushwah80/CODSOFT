# Customer Churn Prediction

This project predicts whether a customer will churn based on demographics and usage behavior using machine learning models such as Logistic Regression, Random Forest, and XGBoost.

---

## Project Structure

├── dataset/
│ └── churn.csv
├── model/
│ └── churn_model.pkl
├── notebook/
│ └── churn_prediction.ipynb
├── requirements.txt
└── README.md


---

## Data Preprocessing

- Dropped identifier columns:
  - RowNumber
  - CustomerId
  - Surname

- Encoded categorical variables:
  - Gender → Label Encoding (Male/Female)
  - Other object columns encoded using LabelEncoder

- Handled missing values if required
- Scaled numerical features for ML models

---

## Models Used

- Logistic Regression  
- Random Forest Classifier  
- XGBoost Classifier  

**Metrics Used:**

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

---

## How to Run

Install dependencies:

pip install -r requirements.txt
Run notebook:

Open the file:

churn_prediction.ipynb

Run all cells.

---

## Dataset

Any Customer Churn dataset from Kaggle (Bank/Telecom Churn dataset).

---

## Conclusion

This project shows:

- How to preprocess data  
- Encode categorical columns  
- Train multiple ML models  
- Compare performance  
- Predict churn effectively  
