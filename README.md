# 🛒 Brazilian E-Commerce Data Analytics (Olist Dataset)

## 📌 Project Overview
This project performs an end-to-end exploratory data analysis (EDA) on the Olist Brazilian E-Commerce dataset. Using a multi-table relational schema containing ~100k orders from 2016 to 2018, the analysis investigates regional revenue distribution, logistics and delivery efficiency, customer review sentiment, payment preferences, and top-performing product categories.

---

## 🛠️ Tools & Technologies Used
* **Python**: Core programming language for analysis
* **Pandas**: Data manipulation, cleaning, datetime parsing, and multi-table relational joins (`pd.merge`)
* **NumPy**: Numerical aggregation and vector operations
* **Matplotlib & Seaborn**: Data visualisations and exploratory charting
* **Jupyter Notebook**: Interactive development environment

---

## 📂 Dataset Architecture
The analysis connects several key tables using relational foreign keys (`order_id`, `customer_id`, `product_id`):
* `olist_orders_dataset.csv` - Order statuses and delivery timestamps
* `olist_order_items_dataset.csv` - Item prices and freight costs
* `olist_customers_dataset.csv` - Customer location details (city/state)
* `olist_order_payments_dataset.csv` - Transaction payment methods and installment counts
* `olist_order_reviews_dataset.csv` - Star ratings (1 to 5) and review timestamps
* `olist_products_dataset.csv` & `product_category_name_translation.csv` - Product metadata and English category mappings

---

## 🔑 Key Business Insights & Findings

### 1. Regional Sales Distribution
* **Southeast Dominance:** São Paulo (`SP`) drives the vast majority of total platform revenue and order volumes compared to all other Brazilian states combined.
* **Logistics Costs:** States in the remote North/Northeast regions experience significantly higher average freight costs relative to product prices.

### 2. Delivery Delays vs. Customer Satisfaction
* **Fulfillment Metrics:** Standard delivery times average around 12–15 days across Brazil.
* **Sentiment Impact:** Orders delivered after the estimated delivery date experience a sharp drop in average customer review scores (dropping from ~4.2 stars down to ~2.1 stars), proving logistics directly impacts customer retention.

### 3. Payment Method Analysis
* **Credit Cards Lead:** Credit cards account for over 75% of total sales volume, followed by *Boleto Bancário* and vouchers.

### 4. Top Product Categories
* **Revenue Drivers:** High-performing categories include **Health & Beauty**, **Watches & Gifts**, **Bed Bath & Table**, and **Computer Accessories**.

---

## 🚀 How to Run the Notebook

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/KIRA832/olist-ecommerce-analytics.git](https://github.com/KIRA832/olist-ecommerce-analytics.git)
   cd olist-ecommerce-analytics

2. Install Dependencies:
    ```bash
    pip install pandas numpy matplotlib seaborn

3. Launch Jupyter Notebook:
    ```bash
    jupyter notebook olist_analysis.ipynb

👤 Author
Rajdeep Das - Data Analyst & Computer Engineering Student

GitHub Profile: KIRA832

Project Repository: olist-ecommerce-analytics