# 💳 Fraud Detection System 🕵️‍♀️
*Machine Learning Project – Catching fraudsters one transaction at a time!* 🚀

---

## 🎯 Why This Project?

Every day, thousands of transactions flow through financial systems – but some of them are **sneaky fraud attempts** 🥷. This project builds a smart system to spot those fraudulent transactions *before* they cause any damage.

✅ Built for **Data Science Interns** to showcase their skills.  
✅ Uses **real-world style data** (~6.3 million rows!) to train machine learning models.

---

## 📊 Dataset at a Glance

| Feature             | Description                                               |
|---------------------|-----------------------------------------------------------|
| `step`              | Time step in hours (1 = first hour, 2 = second hour, ...)|  
| `type`              | Transaction type: CASH-IN, CASH-OUT, TRANSFER, etc.      |  
| `amount`            | Transaction amount.                                      |  
| `oldbalanceOrg`     | Sender's balance before the transaction.                 |  
| `newbalanceOrig`    | Sender's balance after the transaction.                  |  
| `oldbalanceDest`    | Recipient's balance before the transaction.              |  
| `newbalanceDest`    | Recipient's balance after the transaction.               |  
| `isFraud`           | 🚨 Target: 1 = fraud, 0 = legit.                          |  
| `isFlaggedFraud`    | Flag for illegal attempts (>200,000 units).               |

📢 **Class Imbalance Alert:** Fraudulent transactions make up only **0.17%** of the dataset!

---

## 🛠️ How It Works

1. **Data Cleaning & Preprocessing**  
   - Handled missing values, outliers, and encoded transaction types.  
   - Added engineered features like `balanceDiff` to improve detection.

2. **Exploratory Data Analysis (EDA)**  
   - Visualized fraud patterns across transaction types and amounts.  
   - Spotted class imbalance early.

3. **Model Building**  
   - Baseline: Logistic Regression.  
   - Advanced: Random Forest, XGBoost, and LightGBM.  
   - Used weighted losses & tuning for handling rare fraud cases.

4. **Evaluation**  
   - **Metrics:** ROC-AUC, Precision, Recall, F1-Score.  
   - Feature importance plots to explain predictions.

---

## 🏆 Results

| Model              | ROC-AUC | Precision | Recall |
|---------------------|---------|-----------|--------|
| Logistic Regression | 0.92    | 12%       | 78%    |
| XGBoost             | 0.991   | 89%       | 95%    |
| LightGBM            | 🏅 0.993| 91%       | 96%    |

🎉 **Winner: LightGBM** – lightweight, fast, and highly accurate!

---

## 📂 Folder Structure
fraud-detection-project/
├── FraudDetection.ipynb # Full notebook: EDA + modeling
├── FraudDetection_Technical.md # Technical report
├── FraudDetection_Business.md # Stakeholder-friendly report
├── generate_charts.py # Script to make charts
├── charts/ # Saved chart images
├── README.md # This file


---

## 🚀 Quick Start

1. Clone this repo:
   ```bash
   git clone https://github.com/hi-riddhi/fraud-detection-project.git
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Add your dataset: Drop Fraud.csv into the project folder.

Run the notebook:

bash
Copy
Edit
jupyter notebook FraudDetection.ipynb
Make charts:

bash
Copy
Edit
python generate_charts.py
🌟 Highlights
Tackled a real-world imbalanced classification problem.

Built smart ML models (LightGBM, XGBoost) to detect fraud.

Delivered technical & business reports for different audiences.

✨ About Me
Hi, I’m Riddhi! This project was part of my Data Science Internship Portfolio.

💻 Skills used: Python, Pandas, Scikit-learn, LightGBM, Data Visualization.
🌐 GitHub: hi-riddhi


