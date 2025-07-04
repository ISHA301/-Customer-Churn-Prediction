# 📊 Customer Churn Prediction using Python

This project focuses on predicting customer churn using a real-world telecom dataset. The goal is to analyze patterns in customer behavior and identify those likely to leave the service, enabling the business to take proactive retention steps.

---

## 📁 Project Overview

### **Business Context**  
Churn (customer leaving the service) can significantly impact revenue. By analyzing historical customer data, we can understand the characteristics of customers who tend to churn and take action accordingly.

### **Project Goal**
- Use Python for data cleaning, analysis, and predictive modeling  
- Understand key customer attributes that influence churn  
- Build an interpretable churn prediction model using logistic regression  
- Generate actionable business insights from data exploration  

---

## 🛠️ Tools & Libraries Used
- **Python**
- **Pandas**, **NumPy** – Data manipulation  
- **Seaborn**, **Matplotlib** – Data visualization  
- **Scikit-learn** – Model building and evaluation  

---

## ✅ Steps Performed

### 1. **Data Cleaning**
- Loaded the dataset from CSV  
- Converted `TotalCharges` to numeric and dropped rows with missing values  
- Removed unnecessary identifiers like `customerID`  

### 2. **Exploratory Data Analysis (EDA)**
- Visualized churn distribution and customer trends using seaborn and matplotlib  
- Analyzed average values of `tenure`, `MonthlyCharges`, and `TotalCharges` across churned vs non-churned customers  
- Explored the relationship between churn and services like internet type, contract length, and tech support  

### 3. **Feature Engineering**
- Created a new binary column: `Churn_Yes` (1 for Yes, 0 for No)  
- Applied one-hot encoding to convert categorical columns into numerical format using `pd.get_dummies()`  

### 4. **Churn Prediction using Logistic Regression**
- Split the data into training and test sets using an 80-20 split  
- Trained a Logistic Regression model using `class_weight='balanced'` to handle class imbalance  
- Evaluated using accuracy, confusion matrix, and classification report  

---

## 📈 Results
- The model achieved **77% accuracy**, and more importantly, strong **recall** on churned customers  
- Effective for identifying high-risk customers to support retention efforts  

---

## 🔍 Key Insights from the Data
- Customers with short-term contracts, electronic check payments, and no technical support are more likely to churn  
- Churned customers had shorter tenure and higher monthly charges on average  
- Lack of services such as online security and streaming options correlated with churn behavior  

---

## 💼 Recommendations
- Promote longer-term contracts or bundled offers to reduce churn  
- Offer discounts or added value for customers using electronic check payments  
- Target at-risk customers with proactive support, especially those lacking tech support or online security  

---

## 📄 Project Artifacts

- 📘 [Business Requirements Document (BRD)](https://github.com/ISHA301/-Customer-Churn-Prediction/blob/main/Customer_Churn_BRD.docx)  
- 📗 [Functional Requirements Document (FRD)](https://github.com/ISHA301/-Customer-Churn-Prediction/blob/main/Customer_Churn_FRD.docx)  

---

## 📓 Jupyter Notebook
🔗 [Click here to view the full Jupyter Notebook](https://github.com/ISHA301/-Customer-Churn-Prediction/blob/main/Customer_Churn_Prediction.ipynb)
