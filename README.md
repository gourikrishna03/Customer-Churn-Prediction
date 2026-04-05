#  Customer Churn Prediction (Machine Learning Project)

##  Project Overview
This project focuses on predicting customer churn using machine learning techniques. The goal is to identify customers who are likely to leave a telecom service, enabling businesses to take proactive retention actions.

---

##  Dataset
- **Dataset**: Telco Customer Churn Dataset  
- **Records**: 7,000+ customers  
- **Features**: Demographics, services, billing, and contract details  

---

## Problem Statement
Customer churn is a critical problem in the telecom industry. Retaining existing customers is more cost-effective than acquiring new ones.  
This project aims to build a model that can accurately predict which customers are likely to churn.

---

##  Approach

### 1️⃣ Data Preprocessing
- Handled missing values in `TotalCharges`
- Converted categorical features into numerical using:
  - Label Encoding
  - One-Hot Encoding
- Removed irrelevant features (`customerID`)
- Ensured all features are numeric

---

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualized churn distribution
- Identified class imbalance
- Analyzed relationships between features and churn

---

### 3️⃣ Handling Class Imbalance
- Applied **class weighting** to improve churn detection
- Focused on improving **recall for churn class**

---

### 4️⃣ Model Building

#### 🔹 Logistic Regression (Baseline Model)
- Improved recall using `class_weight='balanced'`

#### 🔹 XGBoost (Advanced Model)
- Captured non-linear relationships
- Used `scale_pos_weight` for imbalance handling

---

## Model Performance

| Model                | Recall (Churn) | ROC-AUC |
|---------------------|---------------|--------|
| Logistic Regression | 0.80          | 0.83   |
| XGBoost             | 0.78          | 0.83   |

---

## Key Insights

- Customers using **Fiber Optic Internet** show higher churn  
- **Electronic Check payment method** is a strong churn indicator  
- Customers with **higher monthly charges** are more likely to churn  
- Customers without **bundled services** have lower retention  
- **Senior citizens** show higher churn rates  

---

## 💼 Business Recommendations

- Offer **bundled services** to improve retention  
- Promote **auto-payment methods**  
- Provide **discounts for high-paying customers**  
- Target high-risk customers with **personalized offers**  

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Seaborn, Matplotlib  

---

## 📌 Conclusion
The model successfully identifies high-risk customers with strong recall, helping businesses take proactive steps to reduce churn and improve customer retention.

---

## 🔗 Author
**Gourikrishna T**  
📧 gourikrishna499@gmail.com