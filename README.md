# Olist E-Commerce SQL Analysis

Project Overview

This project analyses the Brazilian **Olist e-commerce dataset** using SQL to explore sales performance, customer purchasing behaviour, and revenue trends. The goal of the analysis is to answer key business questions related to product performance, seller revenue distribution, and overall sales growth.
The dataset contains transactional e-commerce data including orders, products, payments, customers, and reviews. By joining and aggregating these tables, the analysis uncovers insights about how the marketplace performs over time.


Dataset

The dataset used in this project is the **Olist Brazilian E-Commerce Public Dataset** available on Kaggle.
It contains multiple relational tables representing different parts of the e-commerce platform.

Key tables used in the analysis

| Table | Description |
|------|-------------|
| orders | Contains order information including timestamps and delivery dates |
| order_items | Contains individual products within each order |
| order_payments | Contains payment transactions for orders |
| products | Contains product category information |
| customers | Contains customer location data |
| order_reviews | Contains review scores given by customers |


Business Questions Explored

The analysis focuses on answering several business questions:
- How many orders exist in the dataset?
- Which product categories sell the most items?
- Which sellers generate the highest revenue?
- What is the average order value?
- How does revenue change over time?
- Which customers spend the most?
- How often are orders delivered late?
- How do seller order values change between consecutive orders?


SQL Concepts Used

This project demonstrates the use of several important SQL concepts used in real-world data analysis:
- Joins across multiple relational tables
- Aggregations (SUM, COUNT, AVG)
- GROUP BY and HAVING
- Window functions (LAG, RANK)
- Running totals using window functions
- Common Table Expressions (CTEs)
- Creating views for data aggregation
- Handling many-to-many join duplication


Handling Join Duplication

One challenge in the dataset is that the order_payments table contains multiple rows per order due to payment installments.
Joining this table directly with other tables caused row duplication, which impacted revenue calculations.
To resolve this issue, an aggregated view was created to calculate one total payment value per order**.

Dataset is too large to upload
Dataset URL: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce


