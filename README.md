**Fraud Detection System - KTC** 💳🔍

This project implements a robust Fraud Detection System for financial transactions using machine learning techniques, including XGBoost, to classify transactions as fraudulent or non-fraudulent. By analyzing transaction patterns and leveraging advanced models, the system ensures high accuracy and provides actionable insights for financial security.

📚 **Overview**
Fraudulent activities in financial transactions pose a significant risk to businesses and customers. This project addresses this challenge using a supervised learning approach, including data preprocessing, exploratory data analysis (EDA), advanced machine learning models, and evaluation metrics to build an effective fraud detection system.

🔑 **Key Features**

1. Dataset Analysis and Insights
Dataset: The project uses the dataset PS_20174392719_1491204439457_log.csv, containing anonymized financial transaction data with the following attributes:

Transaction Type: CASH-IN, CASH-OUT, DEBIT, PAYMENT, TRANSFER.
Transaction Amount: Numeric values for transaction amounts.
Account Information: Includes nameOrig and nameDest (origin and destination accounts).
Fraud Indicators: Flags for fraud (isFraud) and suspicious transactions (isFlaggedFraud).
Exploratory Data Analysis (EDA):

Distribution of transaction types.
Fraud-to-non-fraud ratio.
Transaction patterns by type and fraud indicators.

2. Data Preprocessing
Verified dataset integrity by checking for null values.
Engineered features to analyze fraud-related patterns, including grouping transactions by type and identifying flagged frauds.
Addressed class imbalance to ensure effective model training.

4. Machine Learning Modeling
Implemented XGBoost (Extreme Gradient Boosting), a powerful and efficient gradient-boosting algorithm, for fraud detection.
Additionally explored Logistic Regression for baseline comparisons.
Split the dataset into training and testing sets using an 80:20 ratio.

6. Evaluation Metrics:
Accuracy Score: Assesses overall correctness of the model.
Precision, Recall, F1-Score: Evaluates performance in fraud classification.
AUC-ROC Curve: Highlights the trade-off between sensitivity and specificity.

7. Results and Insights
XGBoost outperformed Logistic Regression, achieving better precision and recall while minimizing false positives.
Highlighted key transaction features that contribute to fraud detection.
Explored patterns in flagged fraud transactions to improve detection accuracy.

💻 **Tech Stack**

Programming Languages & Tools
Python: For end-to-end development.
Jupyter Notebook: For interactive development and visualization.
Libraries
Data Handling: Pandas, NumPy
Data Visualization: Matplotlib, Seaborn
Machine Learning:
XGBoost: For gradient boosting-based fraud detection.
Scikit-learn: For Logistic Regression and evaluation metrics.
🚀 How to Run
Clone the Repository:

bash
Copy code
git clone https://github.com/Samik123Mit/KTC-Hackathon.git  
Install Dependencies:
Install all required libraries from requirements.txt:

bash
Copy code
pip install -r requirements.txt  
Prepare the Dataset:

Download the dataset: PS_20174392719_1491204439457_log.csv.
Place the dataset in the root directory of the project.
Run the Notebook:
Open the fraud_ktc.ipynb in Jupyter Notebook or any compatible IDE and execute cells sequentially.

📊 **Results and Observations**

EDA Observations:
Fraudulent transactions are concentrated in specific transaction types (e.g., TRANSFER and CASH_OUT).
Fraudulent and non-fraudulent transactions show distinct patterns in origin and destination accounts.
Model Performance:
XGBoost achieved higher precision, recall, and AUC-ROC scores compared to Logistic Regression.
Minimized false positives while ensuring accurate fraud detection.
🛠️ Future Enhancements
Incorporate real-time fraud detection capabilities with optimized inference time.
Experiment with additional ensemble learning models (e.g., Random Forest, LightGBM) for performance improvements.
Address class imbalance using techniques like SMOTE or ADASYN.
Integrate with financial systems for live deployment.
Feel free to explore, contribute, and enhance this project! 🚀
