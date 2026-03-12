# Zepto_inventory_analysis

# Project Background

Zepto is a **quick commerce grocery delivery platform** that delivers products within minutes using dark stores.

As a data analyst, the objective of this analysis was to understand:

- Product pricing strategy
- Discount patterns
- Inventory availability
- Revenue potential across categories


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
