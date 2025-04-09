# 💳 Fraud Transaction Detection

This project focuses on detecting fraudulent financial transactions using machine learning. The dataset simulates real-world banking activity, including both normal and fraudulent transactions. Our goal is to build a predictive model that can help financial institutions detect and prevent fraud efficiently.

---

## 📌 Problem Statement

A financial company is experiencing a rise in fraudulent transactions, damaging its reputation and reducing customer trust. The company seeks a reliable system to detect these transactions in advance and take preventive action.

---

## 🔍 Project Objectives

- Clean and preprocess a large transaction dataset
- Perform exploratory data analysis (EDA) to identify patterns
- Engineer relevant features for better model performance
- Build and evaluate machine learning models for fraud detection
- Provide insights on fraud behavior and suggest prevention strategies

---

## 🧠 Techniques Used

- Data Cleaning (handling null values, outliers, type conversion)
- Feature Engineering (sender/receiver type, transaction patterns)
- Label Encoding
- Machine Learning Models: Logistic Regression, Random Forest, XGBoost
- Model Evaluation: Confusion Matrix, ROC-AUC, Precision, Recall
- Visualization: Power BI for fraud trend analysis

---

## 🧾 Dataset Overview

- **Rows:** 6.3 million+
- **Columns:** 10
- **Features:**
  - `step`: Time step (1 step = 1 hour)
  - `type`: Transaction type (TRANSFER, CASH_OUT, etc.)
  - `amount`: Transaction amount
  - `nameOrig`, `nameDest`: Sender and receiver identifiers
  - `oldbalanceOrg`, `newbalanceOrig`: Sender's balances
  - `oldbalanceDest`, `newbalanceDest`: Receiver's balances
  - `isFraud`: Indicates whether the transaction is fraud
  - `isFlaggedFraud`: Flags illegal large transactions (>200K)

---

## 📊 Key Insights

- All frauds are in **TRANSFER** and **CASH_OUT** types
- Most frauds happen in **CASH_OUT** type
- Fraudulent transactions always involve **customers** on both sides
- **Merchants are rarely or not involved** in fraudulent activities, but limited data makes this inconclusive

---

## 🚀 How to Run

1. Clone this repository
2. Load the dataset (`.csv`)
3. Run the Jupyter Notebook: `fraud_detection.ipynb`
4. Use Power BI dashboard for interactive data insights (optional)

---

## 📁 Project Structure

```
├── fraud_detection.ipynb        # Main analysis and modeling notebook
├── Fraud_Dashboard.pbix         # Power BI dashboard
├── data/
│   └── fraud_data.csv           # Transaction dataset
├── README.md                    # Project documentation
└── requirements.txt             # Python dependencies
```

---

## 📌 Conclusion

This project demonstrates how machine learning can be effectively used to detect fraud and help financial institutions take proactive steps in protecting their systems and customers.
