# Postgresql Practicing Queries

This project contains a collection of **intermediate and advanced SQL queries** written and executed in a **Jupyter Notebook** using a **Contoso-100K sales dataset**.

---

## 📌 Project Objectives

* Practice **real-world SQL analytics queries**
* Cover frequently tested SQL concepts:

  * `CASE WHEN`
  * Data filtering (`WHERE`, `IN`, `BETWEEN`, `LIKE`, `IS NULL`, `REGEXP`)
  * Logical operators (`AND`, `OR`, `NOT`)
  * Aggregations and `HAVING`
  * Window functions
  * CTEs
* Apply SQL to a **fact + dimension (OLAP-style) data model**
* Document solutions clearly for **GitHub portfolio and interviews**

---

## 🧱 Dataset Overview

### ⭐ Fact Table

**`sales`**

* Order-level transactional data
* Measures: quantity, net price, unit cost
* Foreign keys to date, customer, store, product, and currency tables

### 📐 Dimension Tables

* `date` – calendar and time attributes
* `customer` – demographic and geographic data
* `store` – store metadata
* `product` – product hierarchy and pricing
* `currencyexchange` – FX rates by date

---

## 🔗 Schema Relationships

* `sales.orderdate` → `date.date`
* `sales.customerkey` → `customer.customerkey`
* `sales.storekey` → `store.storekey`
* `sales.productkey` → `product.productkey`
* `currencyexchange.date` → `date.date`

---

## 🧪 Topics Covered

### 🟡 Intermediate SQL

* Conditional logic using `CASE WHEN`
* Data filtering with:

  * `WHERE`, `IN`, `BETWEEN`
  * `LIKE`, `IS NULL`
* Logical conditions (`AND`, `OR`)
* Grouping and aggregation
* Business logic translation into SQL

### 🔵 Advanced SQL

* `HAVING` for post-aggregation filtering
* Revenue and profitability analysis
* Customer segmentation (VIP vs Regular)
* Time-based comparisons (YoY, MoM)
* Regex filtering using `REGEXP`
* Multi-condition analytical queries
* CTEs for readable and modular SQL
