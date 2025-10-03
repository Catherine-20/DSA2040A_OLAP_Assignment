# DSA2040A — OLAP Assignment (Fall 2025)
INGABIRE CATHERINE-671041

## 📌 Project Overview
This assignment demonstrates how to design and implement a small OLAP system using **SQLite** and **Pandas** in Jupyter Notebook.  
The goal is to practice different OLAP architectures (ROLAP, MOLAP, HOLAP) and operations (Slice, Dice, Roll-Up, Drill-Down), as well as create simple visualizations.

---

## 📂 Files
- **olap_assignment.ipynb** → Jupyter Notebook with all code, queries, and visualizations.  
- **README.md** → documentation of the project.  

---

## 🗄️ Data Warehouse Schema
We used a simple **star schema**:

### Fact Table
- **sales** (sale_id, date, product_id, quantity, revenue)

### Dimension Tables
- **products** (product_id, category, name, price)  
- **dates** (date, year, quarter, month)  

---

## ⚙️ OLAP Architectures

### 1. ROLAP (Relational OLAP)
Implemented using SQL queries on the SQLite database:
- Average revenue by product category  
- Total sales by year  
- Best-selling product in each category  

### 2. MOLAP (Multidimensional OLAP)
Implemented with **Pandas Pivot Tables** to build cubes:
- Example: Revenue by product category × year  

### 3. HOLAP (Hybrid OLAP)
Combined SQL queries (detail-level data) with Pandas pivot tables (aggregated summaries).

---

## 🔍 OLAP Operations

- **Slice** → Sales for a specific year (e.g. 2024 only).  
- **Dice** → Sales in Q1 2024 for Electronics category.  
- **Roll-Up** → Aggregate from product → category → year.  
- **Drill-Down** → From year → quarter → month.  

---

## 📊 Visualizations
1. **Bar Chart** → Revenue by category  
2. **Bar Chart** → Best-selling product in each category  
3. **Heatmap (optional)** → Category × Year cube  

---

## 🚀 How to Run
1. Clone this repo:  
   ```bash
   git clone https://github.com/Catherine-20/DSA2040A_OLAP_Assignment.git
   cd DSA2040A_OLAP_Assignment
