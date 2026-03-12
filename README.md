# Zepto_inventory_analysis

## Portfolio Project Description
This project demonstrates my ability to use **SQL for real-world business analysis**.  
Using a product dataset from a quick-commerce grocery platform (Zepto), I performed **data exploration, cleaning, and analytical queries in PostgreSQL** to extract insights related to pricing strategies, inventory availability, and category-level revenue potential.

The goal of this project was to simulate the work of a **data analyst supporting business decisions in an e-commerce environment**.

---

# Project Background

Zepto is a **quick commerce grocery delivery platform** that delivers products within minutes using dark stores.

As a data analyst, the objective of this analysis was to understand:

- Product pricing strategy
- Discount patterns
- Inventory availability
- Revenue potential across categories

The SQL queries used in this project can be found here:  
`/SQL/zepto_analysis.sql`

---

# Data Structure

The dataset contains **product-level information**.

Main table: `zepto`

| Column | Description |
|------|------|
| sku_id | Product ID |
| category | Product category |
| name | Product name |
| mrp | Maximum retail price |
| discountPercent | Discount percentage |
| availableQuantity | Available stock |
| discountedSellingPrice | Selling price after discount |
| weightInGms | Product weight |
| outOfStock | Stock availability |
| quantity | Product quantity |

Initial checks included:

- Counting total records
- Checking missing values
- Identifying unique categories
- Analyzing stock availability

---

# Executive Summary

Key findings from the analysis:

1. Several **high-value products are out of stock**, representing possible lost revenue.
2. **Discount strategies vary across product categories**, indicating targeted pricing tactics.
3. Inventory distribution across categories affects potential revenue generation.

---

# Key Insights

## Pricing & Discount Strategy

- Identified the **top 10 products with the highest discounts**.
- Some high-priced products (> ₹500) offer **very low discounts**, which may reduce competitiveness.

---

## Inventory Availability

- Multiple products are **out of stock**, including high-MRP items.
- This suggests potential **inventory management improvements**.

---

## Revenue Potential by Category

Revenue potential was estimated using:

`discountedSellingPrice × availableQuantity`

Some categories contribute significantly more to potential revenue than others.

---

## Product Value Analysis

Price-per-gram analysis was used to identify **best-value products**.

Products were grouped into:

- Low weight (<1000g)
- Medium weight (1000–5000g)
- Bulk (>5000g)

Bulk products generally provide **better value per gram**.

---

# Recommendations

- Improve stock availability for **high-demand and high-value products**.
- Adjust pricing strategies for **expensive low-discount items**.
- Use **high-discount products in promotional campaigns**.
- Optimize inventory distribution to improve **warehouse efficiency**.

---

# Tools Used

- PostgreSQL  
- pgAdmin  
- SQL  

---

# Author

Mariyan Sanduni  
BSc (Hons) Business Information Systems  
University of Sri Jayewardenepura
