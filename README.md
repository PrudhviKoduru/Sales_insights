
# 📊 Retail Sales Analytics – Superstore Dashboard  
**Python + Pandas + Power BI + Kaggle Dataset**

This project analyzes retail sales performance using the popular **Superstore dataset**.  
The workflow follows an industry-style data pipeline:

1. **Data sourced from Kaggle**
2. **Preprocessing and feature engineering in Python (Pandas, NumPy)**
3. **Light transformations in Power Query**
4. **Interactive dashboard built in Power BI**
5. **Cleaned & aggregated datasets exported for reporting**




---

## 📥 1. Data Source (Kaggle)

Dataset used: **Sample Superstore Dataset**  
Kaggle Link: https://www.kaggle.com/datasets/vivek468/superstore-dataset-final

The dataset includes:

- 9,000+ rows  
- Customer, product, shipping, geography  
- Order and ship dates  
- Sales, discount, profit  

---

## 🧼 2. Preprocessing in Python (Pandas + NumPy)

All major cleaning and transformations were done in Python to keep the workflow **reproducible and version-controlled**.

### ✔ Key preprocessing steps:
- Removed duplicates and invalid rows  
- Parsed `Order Date` and `Ship Date`  
- Standardized text fields (City, Region, Category, Product Name, etc.)  
- Created **Year**, **Month**, **Month_Name**  
- Added **Revenue** and **Profit Margin** metrics  
- Generated **monthly aggregated tables** for faster Power BI performance  

### 🔧 Main Script:
[`preprocess_superstore.py`](./preprocess_superstore.py)

### ✔ Output Files:
- `cleaned_data/superstore_cleaned.csv`  
- `cleaned_data/superstore_monthly_sales.csv`

---

## 🔍 3. Light Transformations in Power Query

Only minimal steps were applied:

- Datatype corrections  
- Column renaming  
- Final model adjustments  
- Relationship creation (Date → Sales, Product → Sales, Customer → Sales)

Complex logic was intentionally kept in Python.

---

## 📊 4. Power BI Dashboard
📊 [**Click here to view the interactive dashboard**](https://app.powerbi.com/view?r=eyJrIjoiZjA2NWY4OTgtZmY3MC00NzVmLWJhZmMtMzQ4ODNkZWEyZTkyIiwidCI6ImMzMGI2ZmZmLTRiZGItNGUzOS1hNDY3LWU1ODFkM2QyNTNiYyJ9)

---
## Preview of the Dashboard
![Dashboard Preview](https://github.com/PrudhviKoduru/Sales_insights_Atliq/blob/88daa18605ffbfa4dbec63628d5f9fc99a8377bb/Dashboard/Dashboard%201.png)

The Power BI dashboard visualizes key retail insights:

### **Key Visuals**
- Monthly revenue trend  
- Profit vs. discount analysis  
- Top-performing categories and sub-categories  
- Region-wise performance  
- Customer and product-level KPIs  
- Ship Mode breakdown  
- Profitability segmentation  

### **KPIs Included**
- Total Revenue  
- Total Quantity Sold  
- Total Profit  
- Average Discount  
- Profit Margin  

---

## 🧠 5. Insights Derived

Some example insights:

- Certain sub-categories drive high volume but low profit  
- High-discount regions often show reduced profitability  
- Clear seasonality patterns in quarterly sales  
- Segment-wise differences in customer purchasing behavior  
- West and East regions show strong revenue contribution  

---

## 🚀 6. How to Reproduce This Project

### **1. Install dependencies**
```bash
pip install pandas numpy
