![Zepto SQL Project Banner](https://github.com/yourusername/zepto-SQL-data-analysis-project/assets/banner-image.jpg)

# 🛒 Zepto E-commerce Inventory SQL Analysis

A hands-on SQL project analyzing real-world inventory data inspired by **Zepto**, a fast-growing quick-commerce startup in India. This project simulates actual analyst workflows — from raw data to clean insights — to solve business problems with SQL.

---

## 🔧 Tech Stack & Tools

![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791?logo=postgresql&logoColor=white)
![SQL](https://img.shields.io/badge/Language-SQL-blue)
![pgAdmin](https://img.shields.io/badge/Tool-pgAdmin-336791?logo=postgresql)
![DataCleaning](https://img.shields.io/badge/Step-Data%20Cleaning-orange)
![EDA](https://img.shields.io/badge/Step-Exploratory%20Analysis-yellowgreen)
![BusinessInsights](https://img.shields.io/badge/Step-Business%20Insights-lightgreen)

---

## 📍 Objective

This project was designed to:
- Understand how inventory data works in e-commerce
- Practice data cleaning and transformation using SQL
- Generate actionable insights to support business decisions

---

## 📦 Dataset Summary

The dataset contains product-level inventory scraped from the Zepto app (via Kaggle). Each entry represents a SKU with category, price, stock, discount, and size info.

| Column | Description |
|--------|-------------|
| `name` | Product Name |
| `category` | Product Category (Fruits, Snacks, Beverages...) |
| `mrp` | Maximum Retail Price in ₹ |
| `discountPercent` | Discount percentage |
| `discountedSellingPrice` | Final price after discount |
| `availableQuantity` | Units in stock |
| `weightInGms` | Weight in grams |
| `outOfStock` | Boolean for availability |
| `quantity` | Units per package |

---

## 🚦 Workflow Summary

### 🔹 1. Table Creation  
Created a PostgreSQL table using appropriate data types for each column.

### 🔹 2. Data Import  
Loaded the CSV using `\copy` command in pgAdmin. Handled UTF-8 encoding issues.

### 🔹 3. Data Exploration  
- Viewed sample records  
- Checked for missing/null values  
- Identified in-stock vs out-of-stock items  
- Explored duplicate products (by name and package size)

### 🔹 4. Data Cleaning  
- Removed rows where `MRP` or `Discounted Price` = 0  
- Converted prices from paise to rupees  
- Ensured all numeric and boolean fields were consistent

### 🔹 5. Business Insights (SQL Analysis)  
- 🏷️ Top 10 discounted products  
- 📉 Out-of-stock items with high MRP  
- 💰 Revenue potential by category  
- ❌ Expensive items with low discounts  
- 📊 Average discount per category  
- ⚖️ Price per gram analysis  
- 📦 Grouping by weight: Low, Medium, Bulk  
- 🧮 Inventory weight by category



