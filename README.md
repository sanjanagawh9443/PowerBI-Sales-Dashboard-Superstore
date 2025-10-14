# **Sales Overview Dashboard — Power BI**

## 📘 **Project Overview**

This repository contains the **Sales Overview Dashboard** built in **Power BI** as part of Week 1 learning — focusing on data cleaning, visualization, and basic dashboard design.
The goal is to analyze retail sales performance using KPIs and trends.

---

## 🗂️ **Dataset**

* **Source:** [Kaggle – Superstore Sales Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
* **Format:** CSV / Excel
* **Description:** Contains order details like Sales, Profit, Quantity, Category, and Region.

---

## 💾 **Repository Structure**

```
📦 Sales-Overview-Dashboard
 ┣ 📂 data/ → Raw & cleaned data files (CSV/Excel)
 ┣ 📂 powerbi/ → Power BI project file (.pbix)
 ┣ 📂 assets/ → Dashboard screenshots
 ┣ 📄 README.md → Project documentation
```

---

## 🎯 **Dashboard Features**

* **KPIs:** Total Sales, Total Profit, Total Orders
* **Visuals:**

  * Sales by **Region**, **Category**, **Sub-category**
  * **Monthly Sales Trend** (Line Chart)
  * **Top Products** and **Customers** (Table / Bar Chart)
* **Slicers:**

  * Year
  * Category

---

## 🧹 **Data Cleaning (Power Query Steps)**

1. Removed null or blank rows.
2. Changed data types:

   * Sales & Profit → Decimal
   * Order Date → Date
3. Split columns (if needed).
4. Removed duplicates by `Order ID`.
5. Added calculated columns:

   * `OrderYear = Date.Year([Order Date])`
   * `MonthName = Date.ToText([Order Date], "MMM")`

---

## ⚙️ **DAX Measures Used**

```dax
Total Sales = SUM('Orders'[Sales])
Total Profit = SUM('Orders'[Profit])
Orders Count = DISTINCTCOUNT('Orders'[Order ID])
Average Order Value = DIVIDE([Total Sales], [Orders Count])
Sales LY = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Orders'[Order Date]))
```

---

## 🪄 **How to Use**

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/Sales-Overview-Dashboard.git
   ```
3. Open `Sales_Overview.pbix` file in Power BI.
4. Load dataset from the `data/` folder.
5. Refresh visuals and explore insights.

---

## 🖼️ **Dashboard Preview**

(![Sales Dashboard]()

---

## 👩‍💻 **Contributor**

**Sanjana Gawhande**


