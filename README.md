# 📉 Customer Churn Prediction using Machine Learning

## 🧠 Predicting Customer Retention with AI-Driven Insights
This project implements an end-to-end customer churn forecasting system using machine learning techniques to identify which customers are most likely to leave a telecom service provider. It demonstrates the entire data science workflow—from data preprocessing and exploratory analysis to model evaluation and insight generation.

---

## 📂 Project Structure
```

text
├── eda_customer_churn.ipynb     # Complete analysis, model training & evaluation
├── import_data.py               # Script to download dataset from KaggleHub
├── Telco-Customer-Churn.csv     # Dataset used for analysis
├── README.md                    # Documentation file

````

---

## 💡 Project Overview

### 🎯 Objective
Detect customers likely to discontinue their service and identify the key factors contributing to churn.

### 🔍 Dataset
- **Dataset Name:** Telco Customer Churn  
- **Source:** Kaggle (blastchar/telco-customer-churn)  
- **Rows:** 7,043  
- **Features:** 21 (Demographics, Contract Type, Charges, etc.)

### ⚙️ Tools and Technologies
- **Programming & Visualization:** Python, Pandas, NumPy, Matplotlib, Seaborn  
- **Machine Learning:** Scikit-learn, XGBoost, Random Forest, Logistic Regression  
- **Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC  
- **Environment:** Jupyter Notebook / Google Colab  
- **Dataset Download:** KaggleHub

---

## 🧩 Steps Implemented

### 1️⃣ Data Preprocessing
- Handled missing and invalid entries in `TotalCharges`  
- Converted categorical features using Label Encoding and One-Hot Encoding  
- Scaled numeric columns using `StandardScaler`  

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualized churn distribution and customer demographics  
- Identified churn patterns by contract type, service, and tenure  
- Correlation analysis between monthly/total charges and churn rate  

### 3️⃣ Model Building
Three baseline models were trained and compared:

| Model               | Accuracy | ROC-AUC | Remark                                      |
|--------------------|---------|---------|--------------------------------------------|
| Logistic Regression | 80.7%   | 84.1%   | Best balance between performance & interpretability |
| Random Forest       | 78.9%   | 82.6%   | Strong performance, higher complexity     |
| XGBoost             | 78.5%   | 83.1%   | Optimized boosting model, consistent accuracy |

### 4️⃣ Insights
- Month-to-month contracts show higher churn probability  
- Short-tenure customers are more likely to switch providers  
- High charges correlate with increased churn  
- Customers lacking Online Security or Tech Support churn significantly more  

---

## 📊 Key Results
- Logistic Regression achieved **81% accuracy** and **84% ROC-AUC**  
- Classification reports, confusion matrices, and ROC curves were plotted  
- Generated actionable business insights for customer retention  

---

## 🚀 How to Run

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/customer-churn-prediction.git
cd customer-churn-prediction
````

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Download the dataset

```bash
python import_data.py
```

### 4️⃣ Open the Jupyter notebook

```bash
jupyter notebook eda_customer_churn.ipynb
```

---

## 🔮 Future Enhancements

* Integrate Flask API for real-time churn prediction
* Build interactive Power BI or Streamlit dashboards
* Add SHAP explainability to visualize feature impacts
* Implement auto-retraining pipeline for new customer data

---

## 🧾 Evaluation Summary

| Metric    | Best Model (Logistic Regression) |
| --------- | -------------------------------- |
| Accuracy  | 0.807                            |
| ROC-AUC   | 0.8416                           |
| Precision | 0.66                             |
| Recall    | 0.57                             |
| F1-Score  | 0.61                             |

---

## 🧠 Project Rating

* **Perplexity Pro:** 9/10 — “Industry-level workflow, reliable insights.”
* **ChatGPT (GPT‑5):** 9.1/10 — “Effective structure, high clarity, great business value.”

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss potential updates.

---

## 🪪 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute with attribution.

---

> If you found this project insightful, give it a ⭐ on GitHub!
