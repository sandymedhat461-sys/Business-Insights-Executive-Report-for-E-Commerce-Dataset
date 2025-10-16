# 🛒 E-Commerce Sales & Customer Insights Dashboard

### 📊 End-to-End Data Analytics Project using Python & Power BI  
**Dataset:** Brazilian E-Commerce Public Dataset by Olist (Kaggle)  
**Author:** Sandy Medhat Roshdy  

---

## 🚀 Project Overview
This project provides a **comprehensive analysis of an e-commerce dataset** to uncover sales trends, customer behavior, and product performance.  
It demonstrates the **complete data analytics workflow** — from cleaning and transformation in **Python**, to visualization and insight generation in **Power BI**.

The goal is to support **data-driven business decisions** by presenting key metrics and interactive visualizations.

---

## 🧩 Dataset Description
- **Source:** [Brazilian E-Commerce Public Dataset by Olist – Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- **Files Used:**
  - `olist_orders_dataset.csv`
  - `olist_order_items_dataset.csv`
  - `olist_products_dataset.csv`
  - `olist_sellers_dataset.csv`
  - `product_category_name_translation.csv`
- The datasets were merged and cleaned in Python, then exported as `final_ecommerce_dataset.xlsx` for Power BI analysis.

---

## 🧠 Objectives
- Clean and preprocess the raw sales, product, and customer data  
- Explore sales and delivery patterns using **Exploratory Data Analysis (EDA)**  
- Build an **interactive Power BI dashboard** to visualize:
  - Total sales and revenue by category and region  
  - Monthly and yearly trends  
  - Top customers and sellers  
  - Average delivery time and performance  
- Generate actionable business insights and executive recommendations  

---

## ⚙️ Tools & Technologies
| Tool | Purpose |
|------|----------|
| **Python (Pandas, NumPy)** | Data cleaning, merging, and transformation |
| **Excel** | Quick validation and export for Power BI |
| **Power BI** | Interactive dashboards and visual storytelling |
| **DAX** | KPI creation and business metrics calculation |

---

## 🧾 Data Processing Steps
1. **Import raw CSV files** from Kaggle  
2. **Clean column names** and handle missing data  
3. **Merge datasets** (`orders`, `order_items`, `products`, etc.)  
4. **Feature engineering:** price capping, delivery time, month-year extraction  
5. **Export final dataset** to Excel for Power BI:  

## 📈 Power BI Dashboard
The Power BI dashboard includes:
- **KPIs:**
- Total Revenue  
- Total Orders  
- Average Order Value (AOV)  
- Average Delivery Time  
- **Charts:**
- Revenue by Product Category  
- Orders by State  
- Monthly Sales Trend  
- Top 10 Customers & Sellers  
- Delivery Performance  

📍 The dashboard provides an **executive summary view** for quick decision-making.

---

## 💡 Key Business Insights
- Highest sales from **cool_stuff**, **moveis_decoracao**, and **pet_shop** categories  
- Sales peaks during **November–December**, showing strong seasonal demand  
- **São Paulo** leads in total revenue and order volume  
- **Average delivery time** around 7–9 days indicates strong logistics  
- A small group of loyal, high-value customers contributes a major share of sales  

---

## 🧭 Executive Summary
This project showcases how **data analytics transforms raw e-commerce data into actionable insights**.  
The Power BI dashboard enables stakeholders to:
- Monitor performance metrics in real-time  
- Identify growth opportunities  
- Optimize operations and customer retention strategies  

---

## 🗂️ Repository Structure
📦 E-Commerce-Insights
┣ 📂 powerbi_exports
┃ ┗ 📄 final_ecommerce_dataset.xlsx
┣ 📂 notebooks
┃ ┗ 📄 ecommerce_analysis.ipynb
┣ 📄 README.md
┣ 📄 requirements.txt
┗ 📄 E-Commerce Dashboard.pbix

yaml
Copy code

---

## 🧮 DAX Measures Used
```DAX
Total Sales = SUM('Orders'[price_capped])
Total Orders = DISTINCTCOUNT('Orders'[order_id])
Average Order Value = [Total Sales] / [Total Orders]
Average Delivery Days = AVERAGE('Orders'[delivery_time_days_capped])

## 📬 Contact

Sandy Medhat Roshdy
🎓 Business Information Systems Student – Helwan University
📧 sandymedhat461@gmail.com
🔗 www.linkedin.com/in/sandy-medhat-14827724a
