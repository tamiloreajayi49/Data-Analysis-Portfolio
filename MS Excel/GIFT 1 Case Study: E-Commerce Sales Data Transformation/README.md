# GIFT 1 Case Study: E-Commerce Sales Data Transformation

An end-to-end data cleaning, transformation, and ETL pipeline built with **Power Query (M Code)** and **Microsoft Excel**. This project standardizes raw, inconsistent e-commerce order records and sales targets into an analytics-ready relational data model.

---

## 📌 Project Overview

E-commerce transactional data often arrives with formatting inconsistencies, missing values, and unorganized target metrics. This project demonstrates a structured workflow to **clean, combine, and validate multi-source data** for downstream reporting and analysis.

**Goal:** Transform messy CSV exports into a trusted, analysis-ready dataset that can power dashboards, KPI tracking, and business insights.

---

## 📁 Repository Structure

```text
├── Data/
│   ├── Messy_List_of_Orders.csv    # Customer order headers & shipping locations
│   ├── Messy_Order_Details.csv     # Line-item transactions, amounts, & profits
│   └── Messy_Sales_Target.csv      # Unorganized monthly target metrics
├── Queries/                        # Exported Power Query / M Code scripts
└── README.md                       # Project documentation
```

---

## 🛠️ Key Pipeline Steps

### 1. Automated Folder Ingestion
- Configured **dynamic Power Query folder loads** to automatically combine multiple CSV inputs as new files are added.

### 2. Data Cleaning & Normalization
- Standardized text casing and trimmed whitespace across regions, categories, and product names.  
- Restored missing leading zeros in **Order ID** fields.  
- Unified inconsistent **date formats** and removed null/blank records.  

### 3. Advanced M Code Transformations
- Built **custom M functions** to strip mixed currency symbols (`₹`, `Rs.`, `$`) from amount fields.  
- Parsed raw string fields into clean **numerical data types** (order value, profit, targets).  
- Executed **fuzzy matching** to map and correct misspelled state and city names.  

### 4. Data Integration & Modeling
- Merged **order headers** with **line-item transaction details** on Order ID.  
- Mapped **actual sales** against **monthly sales targets** to enable performance analysis.  
- Designed a simple relational model suitable for further analysis in Excel or Power BI.  

### 5. Quality Assurance Checks
- Validated **schema integrity** across all tables.  
- Checked **row counts** before and after transformations.  
- Verified **referential joins** between orders and order details.  
- Audited and removed **duplicate records**.  

---

## 🧰 Tools & Technologies

- **Microsoft Excel**  
- **Power Query / M Code**  
- **ETL & Data Modeling Principles**  

---

## 📊 Outcomes

- A repeatable, documented ETL process that can be refreshed as new data arrives.  
- Clean, standardized tables ready for:
  - Sales performance analysis  
  - Region/category breakdowns  
  - Actuals vs. target comparisons  
- A practical demonstration of real-world data cleaning and transformation skills.  

---

## 🚀 How to Use This Project

1. Clone or download this repository.  
2. Open the Excel workbook (if included) and refresh the Power Query queries.  
3. Inspect the transformed tables in the **Queries & Connections** pane.  
4. Use the cleaned data for your own analysis, dashboards, or as a template for similar projects.  

---

## 👤 About the Author

**Tamilore Ajayi** – Data Analyst  
📧 Email: tamiloreajayi49@gmail.com
🔗 GitHub: https://github.com/tamiloreajayi49 

---

## 📫 Contact

If you’d like to discuss this project, collaborate on data work, or talk about ETL/analytics:

- **Email:** tamiloreajayi49@gmail.com

---
