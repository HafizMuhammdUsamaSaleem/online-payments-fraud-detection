### Online Payments Fraud Detection

This project builds a machine learning model to detect fraudulent online payment transactions. It uses real-world transactional data and demonstrates effective techniques for handling imbalanced classification problems.

---

### Dataset

- **Source**: [Kaggle – Online Payments Fraud Detection Dataset](https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset)
- **Size**: ~187 MB CSV
- **Records**: 636,262 transactions
- **Features**:
  - `type`: Transaction type (e.g., PAYMENT, TRANSFER)
  - `amount`: Transaction amount
  - `oldbalanceOrg`, `newbalanceOrig`: Sender’s balance before and after
  - `oldbalanceDest`, `newbalanceDest`: Receiver’s balance before and after
  - `isFraud`: Fraud label (1 = fraudulent, 0 = legit)


### Objective

Build and evaluate machine learning models to predict fraudulent transactions using supervised learning techniques. The project focuses on:
- Understanding transaction behavior
- Handling severe class imbalance
- Evaluating model performance beyond accuracy (e.g., precision, recall)


### Tech Stack

- Python 🐍
- Jupyter Notebook
- Data Analysis
- Pandas, NumPy, Seaborn, Matplotlib 📊
- Scikit-learn for ML models 


### Getting Started

1. Clone the repository
```
git clone https://github.com/HafizMuhammdUsamaSaleem/online-payments-fraud-detection.git
cd online-payments-fraud-detection
```
2. Download the dataset

Download the CSV from Kaggle and place it in the root directory.

Ensure the CSV is named ```onlinefraud.csv``` or update the notebook accordingly.

3. Run the notebook
```
jupyter notebook Online_Payments_Fraud_Detection.ipynb

```

### Workflow Summary
##### 1. Data Preprocessing
- Removed irrelevant column: isFlaggedFraud

- Encoded categorical type feature using one-hot encoding

- No null values found

#### 2. Exploratory Data Analysis
- Only ~0.13% of transactions are fraudulent (heavily imbalanced)

- Fraud is most common in TRANSFER and CASH_OUT types

- Fraudulent transactions often have zero recipient balance before and after

#### 3. Model Training
- Logistic Regression

- Decision Tree Classifier

- Random Forest Classifier

#### 4. Evaluation Metrics
- Confusion matrix

- Accuracy, precision, recall, F1-score

- ROC AUC score

