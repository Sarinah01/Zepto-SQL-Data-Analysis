# Zepto Product Analysis (SQL Project)

## Overview
This project performs **data exploration, cleaning, and analysis** on a Zepto product dataset using SQL.  
The goal is to understand product availability, pricing, discounts, inventory distribution, and revenue insights across categories.

---

## Dataset Structure

The dataset is stored in a single table named `zepto`.

### Table Schema
```sql
CREATE TABLE zepto (
    sku_id SERIAL PRIMARY KEY,
    category VARCHAR(120),
    name VARCHAR(150) NOT NULL,
    mrp NUMERIC(8,2),
    discountPercent NUMERIC(5,2),
    availableQuantity INTEGER,
    discountedSellingPrice NUMERIC(8,2),
    weightInGms INTEGER,
    outOfStock BOOLEAN,
    quantity INTEGER
);
