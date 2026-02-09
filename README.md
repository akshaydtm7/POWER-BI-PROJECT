# Financial Expense Optimization Dashboard – Power BI

## 📌 Project Overview
This project focuses on analyzing and optimizing financial expenses for a mid-size enterprise using **Power BI**.  
The dashboard provides clear visibility into department-wise expenses, monthly spending trends, and budget variance to support data-driven decision-making.

---

## 🎯 Objectives
- Monitor department-wise expense distribution  
- Analyze monthly expense trends  
- Identify overspending categories  
- Compare actual expenses against budget  
- Detect departments exceeding budget limits  
- Support cost-control and budgeting decisions  

---

## 🧾 Dataset Description
The dataset contains **12 months of financial expense data** with the following fields:
- Date  
- Month  
- Department (HR, IT, Finance, Operations)  
- Expense Category  
- Expense Amount  
- Budget Amount  

Dummy data is used for analysis purposes.

---

## 🛠 Tools & Technologies
- **Power BI Desktop**
- **Power Query** (ETL & data cleaning)
- **DAX** (Measures and calculations)

---

## 📊 Dashboard Pages
### 1️⃣ Overview
- Total Expenses
- Monthly Average Expense
- Highest & Lowest Spending Departments
- Department-wise expense summary

### 2️⃣ Department Analysis
- Expense distribution by department
- Category-wise expense breakdown
- Department performance insights

### 3️⃣ Trend Analysis
- Monthly expense trends
- Expense growth and fluctuations over time

### 4️⃣ Budget vs Actual
- Actual vs Budget comparison
- Budget variance heat map
- Departments exceeding budget limits

---

## 📐 Key DAX Measures
```DAX
Total Expenses = SUM ( Expenses[Expense Amount] )

Monthly Average Expense =
AVERAGEX (
    VALUES ( Expenses[Month] ),
    [Total Expenses]
)
