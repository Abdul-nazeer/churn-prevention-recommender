# **Churn Prevention Recommender System**

---

## **1. Introduction**
The **Churn Prevention Recommender System** is designed to identify customers at risk of **churn** and provide personalized recommendations to **retain them**. The system uses **machine learning** (CatBoostClassifier) to analyze customer transactions, service usage, and engagement patterns.  

By predicting **churn probability**, the system suggests **targeted retention strategies** such as discounts, loyalty programs, and personalized offers.

---

## **2. Purpose of Churn Prediction**
The primary objective of churn prediction is to detect customers likely to leave and implement strategies to retain them. This helps businesses:  

✅ **Identify at-risk customers** before they leave.  
✅ **Personalize retention strategies** (discounts, special offers, engagement).  
✅ **Increase customer satisfaction & lifetime value (LTV).**  
✅ **Optimize marketing spend** by targeting the right customers.  

---

## **3. Features of the Recommender System**
### **3.1 Data Processing**
- Reads customer data from **Telco-Customer-Churn.csv**.
- Cleans and preprocesses the dataset.
- Handles missing values and applies **feature engineering**.
- Balances the dataset using **SMOTE** (Synthetic Minority Over-sampling Technique).

### **3.2 Churn Prediction Model**
- Uses **CatBoostClassifier** for high-performance churn prediction.
- Trained using **historical customer data**.
- Evaluated using:
  - **Accuracy**
  - **Precision & Recall**
  - **F1 Score**
  - **ROC-AUC Curve**

### **3.3 Personalized Recommendation Engine**
- Uses **cosine similarity** to find similar customers.
- Recommends **targeted retention strategies** such as:
  - **Discount offers** for customers likely to leave.
  - **Personalized product recommendations** based on past behavior.
  - **Engagement campaigns** like loyalty rewards or push notifications.

### **3.4 Real-Time Dashboard**
- Displays **churn probability** for each customer.
- Provides insights on **high-risk customers** and recommended actions.
- **Visualization tools** for tracking churn rates and retention success.

---

## **4. Dataset Description**
The dataset used is **Telco-Customer-Churn.csv**, which contains customer details, subscription plans, and churn labels.

| **Feature**          | **Description** |
|----------------------|----------------|
| **customerID**      | Unique identifier for each customer |
| **gender**          | Male or Female |
| **SeniorCitizen**   | 1 = Yes, 0 = No |
| **Partner**        | Whether the customer has a partner (Yes/No) |
| **Dependents**      | Whether the customer has dependents (Yes/No) |
| **tenure**         | Number of months the customer has stayed |
| **InternetService** | Type of internet service (DSL, Fiber, No) |
| **Contract**        | Customer contract type (Month-to-month, One year, Two years) |
| **MonthlyCharges**  | The amount charged to the customer monthly |
| **TotalCharges**    | Total amount charged to the customer |
| **Churn**          | Target Variable: (Yes/No) |

---

## **5. Installation and Setup**
To run the **Churn Prevention Recommender System**, follow these steps:

### **5.1 Prerequisites**
Ensure you have the following installed:
- Python (>= 3.8)
- Required libraries:
   bash
  pip install pandas numpy scikit-learn xgboost catboost flask imblearn

