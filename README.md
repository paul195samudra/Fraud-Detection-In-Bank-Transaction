# Fraud Detection in Bank Transactions

A machine learning-based fraud detection project that analyzes banking transactions and identifies potentially fraudulent activities using supervised learning, unsupervised anomaly detection, and rule-based risk analysis.

## 📌 Project Overview

Fraud detection is one of the most important applications of machine learning in the banking and financial sector. This project focuses on identifying fraudulent transactions by analyzing historical banking transaction data and discovering patterns associated with suspicious activities.

The project explores multiple fraud detection techniques, including:

* Exploratory Data Analysis (EDA)
* Data preprocessing
* Feature engineering
* Handling imbalanced datasets
* Supervised machine learning
* Unsupervised anomaly detection
* Rule-based fraud risk scoring
* Fraud probability prediction
* Model evaluation

The main objective is to develop a system capable of identifying suspicious transactions and supporting intelligent fraud monitoring.

---

## 🚀 Key Features

* Analyze historical banking transaction data
* Identify patterns in fraudulent and legitimate transactions
* Analyze fraud based on transaction type and channel
* Analyze time-based transaction behavior
* Engineer meaningful fraud-related features
* Handle imbalanced datasets using SMOTE
* Train supervised machine learning models
* Detect unusual transactions using anomaly detection
* Generate fraud probability scores
* Calculate transaction risk scores
* Identify high-risk transactions
* Evaluate model performance using multiple metrics

---

## 🧠 Machine Learning Models

### Random Forest

A Random Forest classifier is used to learn patterns from historical labeled transaction data and classify transactions as fraudulent or legitimate.

### XGBoost

XGBoost is used for high-performance classification of structured banking transaction data. It also provides fraud probability predictions and feature importance analysis.

### Isolation Forest

Isolation Forest is used for unsupervised anomaly detection. It identifies transactions that significantly differ from normal transaction behavior.

### Rule-Based Risk Scoring

A custom risk scoring approach is used to evaluate suspicious transaction behavior based on different risk factors, such as:

* Previous fraud history
* Unusual transaction time
* International transactions
* New merchants
* High transaction amounts
* Failed transaction attempts
* High daily transaction frequency

---

## ⚖️ Handling Imbalanced Data

Fraud detection datasets are generally highly imbalanced because legitimate transactions significantly outnumber fraudulent transactions.

To address this issue, the project uses:

**SMOTE (Synthetic Minority Over-sampling Technique)**

SMOTE generates synthetic examples of the minority fraud class to improve the model's ability to learn fraudulent transaction patterns.

---

## 🔄 Fraud Detection Workflow

```text
Banking Transaction Dataset
            │
            ▼
    Data Preprocessing
            │
            ▼
 Exploratory Data Analysis
            │
            ▼
    Feature Engineering
            │
            ▼
 Handle Class Imbalance
          (SMOTE)
            │
            ▼
    Machine Learning Models
    ┌────────┼────────┐
    ▼        ▼        ▼
Random    XGBoost  Isolation
Forest             Forest
            │
            ▼
   Fraud Probability &
     Risk Score
            │
            ▼
Normal / Suspicious / Fraud
```

---

## 📊 Dataset Features

The project uses banking transaction-related features such as:

* Transaction ID
* Transaction amount
* Account balance
* Credit score
* Transaction hour
* Transaction type
* Transaction channel
* KYC status
* Previous fraud count
* Failed transaction count
* Daily transaction count
* International transaction status
* Unusual transaction time
* Fraud label

---

## 📁 Project Structure

```text
Fraud-Detection-In-Bank-Transaction/
│
├── Fraud_Detection_in_Bank_Transactions.ipynb
├── New_dataset_Of_a_bank_in_India_.ipynb
├── V>_2_0(fraud_Detection).ipynb
└── README.md
```

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Data Processing

* Pandas
* NumPy

### Data Visualization

* Matplotlib
* Seaborn

### Machine Learning

* Scikit-learn
* XGBoost
* Imbalanced-learn

### Techniques

* Random Forest
* XGBoost
* Isolation Forest
* SMOTE
* Feature Importance Analysis

---

## 📦 Installation

Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn scipy joblib
```

---

## ▶️ How to Run

### Using Google Colab

1. Open any notebook in Google Colab.
2. Upload the required dataset.
3. Update the dataset path in the notebook.
4. Run the notebook cells sequentially.

Example:

```python
import pandas as pd

df = pd.read_csv("path/to/your/dataset.csv")
```

### Using Jupyter Notebook

Clone the repository:

```bash
git clone https://github.com/paul195samudra/Fraud-Detection-In-Bank-Transaction.git
```

Navigate to the project directory:

```bash
cd Fraud-Detection-In-Bank-Transaction
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Then open any notebook and run the cells.

---

## 📈 Model Evaluation

The machine learning models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC Score
* Confusion Matrix
* Classification Report

In fraud detection, **Recall and F1-Score are especially important** because failing to identify a fraudulent transaction can have serious financial consequences.

---

## 🔍 Example Prediction

A trained model can analyze a new banking transaction and generate a fraud prediction.

```text
New Transaction
      │
      ▼
Feature Processing
      │
      ▼
Fraud Detection Model
      │
      ▼
Fraud Probability: 0.87
      │
      ▼
Prediction: Fraud
```

Example:

```text
Predicted Label: Fraud
Fraud Probability: 0.87
```

---

## 🔮 Future Improvements

The project can be extended with:

* Real-time transaction monitoring
* Flask or FastAPI deployment
* Real-time transaction streaming
* Database integration
* Fraud detection API
* Fraud analyst dashboard
* Explainable AI using LIME
* Customer behavioral profiling
* Model drift detection
* Online learning
* Automated fraud alerts
* Manual review workflow
* Hybrid machine learning and rule-based detection

---

## 🎯 Future Vision

The long-term goal of this project is to build a real-time intelligent banking fraud detection system.

The system will:

1. Receive a new transaction.
2. Analyze the transaction in real time.
3. Compare it with historical customer behavior.
4. Generate a fraud probability and risk score.
5. Automatically approve low-risk transactions.
6. Block or flag high-risk transactions.
7. Send suspicious transactions for further investigation.

---


## 📄 License

This project is developed for educational, research, and experimental purposes at the period of my internship.
