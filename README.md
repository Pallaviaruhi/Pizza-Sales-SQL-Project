# 🍕 Pizza Sales SQL Project

## 📋 Project Overview

This SQL project is built using real-world-style pizza sales data from a pizza store. The goal is to analyze ordering patterns, revenue, customer preferences, and overall business performance using SQL queries in Microsoft SQL Server Management Studio (SSMS).

We worked with 4 main datasets:

* **orders.csv**: Order date and time
* **order\_details.csv**: Pizzas ordered in each order
* **pizzas.csv**: Size and price of each pizza
* **pizza\_types.csv**: Type, name, and ingredients of pizzas

---

## ⚙️ Technologies Used

* SQL Server Management Studio (SSMS)
* SQL Queries (JOINS, GROUP BY, aggregate functions, CTEs)

---

## 🧱 Project Structure

### 1. **Database and Table Creation**

We created a SQL database and defined tables for orders, order\_details, pizzas, and pizza\_types.

### 2. **Data Import**

We imported data from `.csv` files using  `BULK INSERT`.

### 3. **Data Cleaning**

Handled errors like:

* Truncation issues with sizes like XL/XXL → Fixed by changing column size from `CHAR(1)` to `VARCHAR(3)`
* Skipped corrupted rows and reloaded only valid data

---

## 📊 Key Insights & Analysis

### 🍕 Total Orders
📦 **21,350 orders** were placed in total.  
> Shows the restaurant's overall order volume.

---

### 💰 Total Revenue
💵 The store earned **$817,860.05** overall.  
> Sum of all pizza prices × quantity sold.

---

### 🧀 Highest-Priced Pizza
👑 **The Greek XXI** costs **$35.95**, making it the most expensive pizza.  
> A candidate for premium promotions.

---

### 📏 Most Popular Size
📊 **Large (L)** pizzas were ordered the most — **18,526 times**.  
> Indicates customer preference for larger servings.

---

### 📆 Average Daily Orders
📈 On average, **138 pizzas** were ordered **per day**.  
> Useful for daily stock & staff planning.

### ⚡ Intermediate-Level Analysis

* **Total Quantity by Category:**

  * Classic: 13,529
  * Veggie: 11,649
  * Supreme: 11,987
  * Chicken: 11,050
  * Mushroom: 1,359

* **Order Distribution by Hour:**

  * Peak order times are between 12 PM to 3 PM and 6 PM to 9 PM.

* **Pizzas by Category:**

  * Veggie pizzas are most varied (27 types).
  * Mushroom has only 3 types.

* **Top 3 Pizzas by Revenue:**

  1. The Thai Chicken Pizza – ₹43,434.25
  2. The Barbecue Chicken Pizza – ₹42,768.00
  3. The California Chicken Pizza – ₹41,409.50

### 🧠 Advanced Insights

* **% Contribution to Total Revenue:**

  * Top pizzas contribute 5–6% each.
  * Revenue is evenly distributed among top sellers.

* **Cumulative Revenue Over Time:**

  * Shows business growth and trends across the year.

* **Top 3 Revenue-Generating Pizzas by Category:**

  * Veggie: The Four Cheese Pizza
  * Classic: The Classic Deluxe Pizza
  * Chicken: The Thai Chicken Pizza
  * Mushroom: The Pepperoni

---

## 💡 Business Takeaways

* **Focus on Classic & Chicken pizzas** — they are consistent top performers.
* **XL and L sizes are preferred** — might consider promoting combo deals.
* **Afternoon & evening** hours are busiest — staffing and promotions can be aligned.
* **Popular pizzas should be regularly stocked** and new variations in those categories can be explored.

---

