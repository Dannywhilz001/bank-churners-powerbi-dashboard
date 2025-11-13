# 🏦 Bank Churners Analysis Dashboard

### 📊 Overview
The **Bank Churners Analysis Dashboard** is a comprehensive Power BI project that provides a detailed analysis of **customer churn behavior** in a financial institution.  
The dashboard focuses on identifying churn drivers, quantifying financial impacts, and helping decision-makers design effective **customer retention strategies**.

This project demonstrates how Power BI can transform raw data into actionable insights using **data modeling**, **DAX measures**, and **interactive visualizations**.

---

## 🎯 Business Objective

Customer churn is a critical challenge in the banking industry — it leads to substantial revenue loss and increases the cost of customer acquisition.  
This dashboard is designed to help stakeholders:

- Understand **why customers leave** (churn drivers)  
- Identify **high-risk segments**  
- Quantify **total revenue loss** and **revenue at risk**  
- Formulate data-backed **retention strategies**

---

## 🧩 Dataset Information

The dataset used for this project is based on the **Bank Churners dataset** (widely available on Kaggle and other open data platforms).

It contains attributes related to:
- Customer demographics (Gender, Age, Education, Marital Status)
- Financial information (Credit Limit, Transaction Amount)
- Card usage behavior (Card Category, Transaction Count)
- Customer churn status (Attrited or Existing)

---

## ⚙️ Tools & Technologies

| Tool | Purpose |
|------|----------|
| **Power BI Desktop** | Dashboard design, data visualization, and DAX calculations |
| **Microsoft Excel / CSV** | Data cleaning and preprocessing |
| **DAX (Data Analysis Expressions)** | Creating custom KPIs and calculated measures |
| **Power Query Editor** | Data transformation and modeling |

---

## 📈 Key Metrics & KPIs

| Metric | Description |
|--------|--------------|
| **Churn Rate %** | Percentage of customers who have churned |
| **Total Revenue Loss** | Total financial loss due to customer attrition |
| **High-Risk Customers** | Customers showing likelihood to churn based on behavior |
| **Revenue at Risk** | Potential loss from customers with high churn probability |
| **Total Transaction Amount** | Overall transaction volume |
| **Average Credit Limit** | Average credit exposure across customer groups |

---

## 🖥️ Dashboard Pages

### 🧭 1️⃣ Customer Churn Overview

- Displays **Churn Rate %, Total Revenue Loss, and High-Risk Customers**
- Breakdown of:
  - Churned vs Retained Customers  
  - Churn Rate by Card Category  
  - Churn Distribution by Gender and Education Level  

📸 **Screenshot:**  
![Dashboard 1](https://ibb.co/1YGz3YHr)

---

### 🧩 2️⃣ Demographic & Income Insights

- Analysis of customer churn segmented by:
  - **Income Category**
  - **Marital Status**
  - **Customer Age**

These visuals highlight which income and demographic segments are most likely to churn.

📸 **Screenshot:**  
![Dashboard 2](https://ibb.co/j9JQMJ2T)

---

### 💰 3️⃣ Financial Insights

- KPIs: **Total Revenue Loss**, **Revenue at Risk**, **Total Transaction Amount**
- Breakdown by:
  - **Average Transaction Amount by Customer Status**
  - **Average Credit Limit by Customer Status**

This section links customer churn to direct financial implications.

📸 **Screenshot:**  
![Dashboard 3](https://ibb.co/yn5Lwz9B)

---

## 🧮 Sample DAX Measures

Below are some of the key DAX expressions used in this report:

```DAX
-- Calculate Churn Rate
Churn Rate % = 
DIVIDE(
    COUNTROWS(FILTER(Customer, Customer[Attrition_Flag] = "Attrited Customer")),
    COUNTROWS(Customer),
    0
)

-- Calculate Total Revenue Loss
Total Revenue Loss = 
SUMX(
    FILTER(Customer, Customer[Attrition_Flag] = "Attrited Customer"),
    Customer[Revenue]
)

-- Identify High Risk Customers
High Risk Customers = 
COUNTROWS(FILTER(Customer, Customer[Churn Risk] = "High"))
````

---

## 💡 Insights & Observations

1. **Platinum and Gold Card** holders show higher churn rates, indicating potential dissatisfaction or competition influence.
2. **Customers with annual income below $60K** are most prone to churn, revealing affordability or service-value gaps.
3. **Single and Divorced** individuals have higher churn rates than Married ones — possible due to less engagement or financial volatility.
4. Younger customers (<35 years) show **moderate churn but lower transaction values**, implying potential future risk.
5. Retained customers have **significantly higher transaction volumes** and **credit limits** — crucial for long-term profitability.

---

## 🚀 How to Use

1. Clone or download this repository:

   ```bash
   git clone https://github.com/<Dannywhilz001>/bank-churners-powerbi-dashboard.git
   ```
2. Open the `Bankchunners.pbix` file using **Power BI Desktop**.
3. Explore all visuals and interact with filters/slicers to uncover insights.

---

## 📂 Folder Structure

```
📦 Bank-Churners-PowerBI-Dashboard
 ┣ 📊 Bankchunners.pbix
 ┣ 🖼️ bankchunners dashboard 1.PNG
 ┣ 🖼️ bankchunners dashboard 2.PNG
 ┣ 🖼️ bankchunners dashboard 3.PNG
 ┗ 📘 README.md
```

---

## 🧠 Learning Outcomes

* Mastered **data modeling** and **relationship building** in Power BI.
* Developed **DAX measures** for KPIs and churn analytics.
* Created professional **Power BI dashboards** for storytelling.
* Enhanced understanding of **customer churn dynamics** in the banking sector.

---

## 🏁 Conclusion

This Power BI project demonstrates how analytical dashboards can empower financial institutions to:

* Identify **at-risk customers**
* Quantify **financial losses**
* Improve **retention strategies** through data-driven insights

The **Bank Churners Dashboard** transforms raw data into business intelligence for better strategic planning.

---

## 👨‍💻 Author

**Oladotun Olawale**
📧 [oladotunolawale29@yahoo.com]
🌐 [http://www.linkedin.com/in/oladotun-olawale]

---

## 🏷 GitHub Topics

`#powerbi` `#data-analytics` `#dashboard` `#customer-churn` `#business-intelligence` `#finance` `#dax` `#banking` `#visualization`

