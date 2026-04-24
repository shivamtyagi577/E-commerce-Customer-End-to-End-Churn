# E-commerce-Customer-End-to-End-Churn
This project analyzes customer churn data from an e‑commerce company to identify customers who are likely to stop using the platform. By understanding behavioral patterns and customer characteristics, the goal is to build a machine learning model that enables proactive customer retention strategies.


# 📊 E‑Commerce Customer Churn Analysis

## 📁 Dataset Overview

This project uses a **customer‑level e‑commerce dataset** designed to analyze and predict **customer churn**, i.e., whether a customer stops using the service.

Each record represents **one customer**, with features describing:

- Demographics  
- Engagement and usage behavior  
- Purchase and transaction history  
- Satisfaction levels and complaints  
- Incentive usage (coupons and cashback)  
- Logistics and delivery‑related factors  

The dataset supports both **business analysis** and **machine learning modeling**.

---

## 🎯 Project Objectives

- Perform **Exploratory Data Analysis (EDA)** to understand customer behavior  
- Identify **key drivers of customer churn**  
- Build **binary classification models** to predict churn  
- Generate **business‑oriented insights** to support customer retention strategies  

---

## 📂 Dataset Structure

The Excel file contains **two sheets**:

### 📄 Sheet 1: `Data Dict` (Data Dictionary)
- Describes column names and business meaning  
- Used only for **documentation**  
- ❌ Not used for modeling  

### 📄 Sheet 2: `E Comm` (Main Dataset)
- Used for **EDA and machine learning**
- **Rows:** One row per customer  
- **Columns:** Customer attributes, behavioral metrics, and churn status  
- **Granularity:** Customer‑level snapshot  

---

## 🎯 Target Variable

### `Churn`

| Value | Meaning |
|------|--------|
| 1 | Customer churned |
| 0 | Customer retained |

✅ This defines the problem as a **binary classification task**.

---

## 🧩 Feature Description

### A. Customer Identity

| Column | Description |
|------|------------|
| CustomerID | Unique identifier for each customer |

⚠️ Used only for identification and **excluded from modeling**.

---

### B. Demographic Features

| Feature | Description |
|--------|------------|
| Gender | Customer gender (Male / Female) |
| MaritalStatus | Single / Married / Divorced |
| CityTier | City classification (Tier 1 = metro, Tier 3 = non‑metro) |

Used to identify **churn patterns across customer segments**.

---

### C. Engagement & Usage Behavior

| Feature | Description |
|--------|------------|
| Tenure | Number of months customer has been associated with the company |
| HourSpendOnApp | Average hours spent on app or website |
| NumberOfDeviceRegistered | Number of devices registered by the customer |
| DaySinceLastOrder | Days since the customer placed the last order |

These are **strong churn indicators**, reflecting engagement and inactivity.

---

### D. Purchase & Transaction Behavior

| Feature | Description |
|--------|------------|
| OrderCount | Number of orders placed in the last month |
| PreferedOrderCat | Most frequently ordered product category |
| OrderAmountHikeFromlastYear | Percentage increase in spending compared to last year |

Used to analyze **purchase intensity and growth trends**.

---

### E. Satisfaction & Service Quality

| Feature | Description |
|--------|------------|
| SatisfactionScore | Customer satisfaction rating |
| Complain | Whether the customer raised a complaint (0 = No, 1 = Yes) |

⚠️ These are **critical churn drivers** influencing customer retention.

---

### F. Logistics & Location Features

| Feature | Description |
|--------|------------|
| WarehouseToHome | Distance between warehouse and customer residence |
| NumberOfAddress | Number of addresses linked to the customer |

These features directly impact **delivery experience and logistics efficiency**.

---

### G. Incentives & Promotions

| Feature | Description |
|--------|------------|
| CouponUsed | Number of coupons used in the last month |
| CashbackAmount | Average cashback received |

Used to evaluate **loyalty programs and promotional effectiveness**.

---

### H. Payment & Access Preferences

| Feature | Description |
|--------|------------|
| PreferredPaymentMode | Credit Card, Debit Card, UPI, COD, etc. |
| PreferredLoginDevice | Mobile phone, computer, etc. |

Useful for **UX improvement, payment optimization, and platform strategy**.

---

## 🧪 Data Type Summary

| Data Type | Examples |
|----------|---------|
| Categorical | Gender, CityTier, PreferredPaymentMode |
| Numerical (Discrete) | OrderCount, CouponUsed |
| Numerical (Continuous) | HourSpendOnApp, CashbackAmount |
| Binary | Churn, Complain |

✅ Suitable for models such as:
- Logistic Regression  
- Random Forest  
- XGBoost  
- AutoML frameworks  

---

## ⚠️ Data Quality Considerations

Common observations in this dataset:

- Missing values (e.g., `WarehouseToHome`, `Tenure`)
- Class imbalance (`Non‑Churn > Churn`)
- Outliers in:
  - `CashbackAmount`
  - `HourSpendOnApp`
  - `DaySinceLastOrder`

➡️ Data preprocessing is required before modeling.

---

## 💼 Why This Dataset Is Ideal for a Portfolio

- ✅ Real‑world customer churn problem  
- ✅ Business‑driven feature set  
- ✅ Strong EDA and visualization potential  
- ✅ Clear modeling objective  
- ✅ Supports end‑to‑end ML pipelines  
---
