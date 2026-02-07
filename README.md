# 🛒 Zepto E-commerce SQL Data Analyst Portfolio Project

Based on an e-commerce inventory dataset that was scraped from Zepto, one of India's fastest-growing quick-commerce businesses, this is a comprehensive, real-world data analyst portfolio project. From exploring raw data to conducting business-focused data analysis, this project mimics actual analyst procedures.

---

## 📌 Project Overview
The goal is to simulate how actual data analysts in the e-commerce or retail industries work behind the scenes to use SQL to:
* ✅ **Set up** a messy, real-world e-commerce inventory database
* ✅ **Perform** Exploratory Data Analysis (EDA) to explore product categories, availability, and pricing inconsistencies
* ✅ **Write** business-driven SQL queries to derive insights around pricing, inventory, stock availability, revenue and more

---

## 📁 Dataset Overview
The dataset came from Zepto's official product listings and was first scraped from Kaggle. It resembles what you would normally find in an actual e-commerce inventory system.

A product's distinct SKU (Stock Keeping Unit) is represented by each row. Because the same product may appear more than once in various packaging sizes, weights, discounts, or categories to increase visibility—exactly like genuine catalog data appears—there are duplicate product names.

### 🧾 Columns:
| Column | Description |
| :--- | :--- |
| **sku_id** | Unique identifier for each product entry (Synthetic Primary Key) |
| **name** | Product name as it appears on the app |
| **category** | Product category like Fruits, Snacks, Beverages, etc. |
| **mrp** | Maximum Retail Price (originally in paise, converted to ₹) |
| **discountPercent** | Discount applied on MRP |
| **discountedSellingPrice** | Final price after discount (also converted to ₹) |
| **availableQuantity** | Units available in inventory |
| **weightInGms** | Product weight in grams |
| **outOfStock** | Boolean flag indicating stock availability |
| **quantity** | Number of units per package (mixed with grams for loose produce) |

---

## 🔍 Data Exploration
* Counted the total number of records in the dataset
* Viewed a sample of the dataset to understand structure and content
* Checked for null values across all columns
* Identified distinct product categories available in the dataset
* Compared in-stock vs out-of-stock product counts
* Detected products present multiple times, representing different SKUs

---

## 🧹 Data Cleaning
* Identified and removed rows where MRP or discounted selling price was zero
* Converted **mrp** and **discountedSellingPrice** from paise to rupees for consistency and readability

---

## 📊 Business Insights
* Found **top 10 best-value products** based on discount percentage
* Identified **high-MRP products** that are currently out of stock
* Estimated **potential revenue** for each product category
* Filtered **expensive products** (MRP > ₹500) with minimal discount
* Ranked **top 5 categories** offering highest average discounts
* Calculated **price per gram** to identify value-for-money products
* Grouped products based on weight into **Low, Medium, and Bulk** categories
* Measured **total inventory weight** per product category
