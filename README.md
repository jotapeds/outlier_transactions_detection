# Outlier Transactions Detection

## Context
### This project adresses a real-world challenge from a Itaú's Hackathon I was part in October 2024.
___
The goal was to develop an anomaly detection system for financial transactions to reduce the daily manual volume of manual approvals that complience officersd needed to process. Ensuring that only approvals deviating from the account's normal behavior would require manual review by the team.

This project uses a publicly available dataset from Kaggle (Synthetic Financial Datasets For Fraud Detection) to replicate the original project core's ideas. 

### 📝 Resume
___
1. Processes millions of account transactions
2. Identifies unusual patterns specific to each account's behavior
3. Flags only suspicious transactions for manual review by officers
4. Reduces approval workload by 90%+ while maintaining anomaly detection accuracy

### 📚 Data & Libs Used
___
* [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/datasets/ealaxi/paysim1/data)
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Scikit-learn
* Scipy

### 🔨  Data prep
___
* Filtered only _Debt_ and _Payment_ category 
* Dropped _isFraud_ and _isFlaggedFraud_
* Transformed _step_ in _week_, _day_ and _hour_

### 📊 Analysis
___
Graths Plot for:
* Amout Distribution
* Time Pattern
* Balance vs Transaction Amount
* Weekly frequency

### 🧠 Training'
___
1. Elbow Method for selecting the optimal number of clusters
2. Split Accounts using K-Means
3. Anomaly identification using Isolation Forest
4. PCA 2D and 3D to select ideal tree impurity   

### 🎯 Results
___
The real Model was able to reduce manual validation by 95%.

❗ All Impurities were set to 1% in this example, but it is possible to fine-tune in the cofigs of the model.  
