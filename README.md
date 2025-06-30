

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

The dataset contains product-level inventory scraped from the Zepto app (via Kaggle).Each row corresponds to a product SKU (Stock Keeping Unit) and includes pricing, weight, availability, and discount information.

| Column                  | Description                                      |
|-------------------------|--------------------------------------------------|
| `Category`              | Product category (e.g., Fruits, Beverages)       |
| `name`                  | Product name                                     |
| `mrp`                   | Maximum Retail Price (in paise, needs ₹ convert) |
| `discountPercent`       | Discount applied on the product (%)              |
| `discountedSellingPrice`| Price after discount (in paise)                  |
| `availableQuantity`     | Units available in stock                         |
| `weightInGms`           | Weight of the product in grams                   |
| `outOfStock`            | Boolean flag for stock status                    |
| `quantity`              | Units per package or loose grams                 |
---
## 📊 Project Workflow

### 🔹 1. Table Creation  
Created a structured PostgreSQL table with correct data types for each column.

### 🔹 2. Data Import  
Used `\copy` in pgAdmin to import the UTF-8 formatted CSV file.

### 🔹 3. Data Exploration  
- Viewed first few rows and structure  
- Counted in-stock vs out-of-stock items  
- Found nulls and zero-price anomalies  
- Explored category-level product counts

### 🔹 4. Data Cleaning  
- Removed records where MRP or selling price = 0  
- Converted paise to ₹ for better readability  
- Checked and handled inconsistent quantity fields

### 🔹 5. Business-Oriented SQL Queries  
- Top 10 products with highest discounts  
- Out-of-stock products with highest MRP  
- Estimated revenue potential by product category  
- Average discount per category  
- Price per gram analysis to detect value-for-money products  
- Total inventory weight grouped by category  
- Classified products into weight buckets (Low, Medium, Bulk)

---


