# 🛒 Brazilian E-Commerce by Olist — Data Analysis & Delivery Delay Prediction Project

This project analyzes real transaction data from the Brazilian e-commerce platform Olist.  
It performs Exploratory Data Analysis (EDA) and builds a machine learning model to predict delivery delays.

<br />

## 📌 Business Problem

- As delivery delays increase, customer satisfaction and review scores decrease.
- Dissatisfied customers are more likely to churn and avoid repeat purchases.
- Ultimately, this negatively impacts overall revenue and brand reputation.

<br />

## 📂 Dataset

[Kaggle — Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

| File Name                               | Description                           |
| --------------------------------------- | ------------------------------------- |
| `olist_orders_dataset.csv`              | Order information and delivery dates  |
| `olist_order_items_dataset.csv`         | Order items and shipping costs        |
| `olist_order_payments_dataset.csv`      | Payment methods and amounts           |
| `olist_order_reviews_dataset.csv`       | Customer reviews and response times   |
| `olist_customers_dataset.csv`           | Customer location information         |
| `olist_sellers_dataset.csv`             | Seller location information           |
| `olist_products_dataset.csv`            | Product categories and attributes     |
| `olist_geolocation_dataset.csv`         | Geolocation based on zip codes        |
| `product_category_name_translation.csv` | Portuguese → English category mapping |

<br />

## 🔄 Analysis Pipeline

```
Data Loading → Data Cleaning → Feature Engineering → Data Merging
   → EDA (Customer / Review / Time / Region) → Predictive Modeling
```

<br />

## 🚀 Run in Colab

- [EDA Notebook](https://colab.research.google.com/drive/1NtxazEaJbC-KfJV5YVfxUDZI3u5ouuGp?usp=sharing)
- [Modeling Notebook](https://colab.research.google.com/drive/1osr5Wpcb7yzx4sWzYsHRFS13on_notTy?usp=sharing)

<br />

## 📊 Exploratory Data Analysis (EDA)

#### 1. Customer Analysis

- Approximately 96.88% of customers are first-time buyers
- New customers contribute the majority of revenue, making retention a key challenge

#### 2. Review Analysis

- Around 80% of customers leave positive reviews (4 stars or higher)
- Orders with delayed delivery have significantly lower average review scores compared to on-time deliveries

#### 3. Regional Analysis

- Delivery delays are most frequent between sellers in São Paulo (SP) and customers in the Southeast region
- High transaction volume leads to a higher absolute number of delays
- Delays are concentrated in specific seller-customer region combinations

#### 4. Time-based Analysis

- Order volume peaked in November 2017
- Delivery delays were highest in March 2018
- Tuesdays show the highest number of orders and delays, indicating early-week logistics bottlenecks

<img width="1274" height="703" alt="image" src="https://github.com/user-attachments/assets/61ade9ae-35ac-4bf5-88df-d8d7929e5e6e" />

## 🤖 Machine Learning (Predictive Modeling)

We predict delivery delay (`is_late`) as a binary classification problem.

- Target: `is_late` (0 = On-time, 1 = Delayed)
- Problem Type: Binary Classification
- Objective: Detect delivery delay risk at the order stage to support operational decision-making

<br />

## 💡 Business Insights

| Area       | Insight                                                                        |
| ---------- | ------------------------------------------------------------------------------ |
| Customer   | Low retention rate (3.12%) → need stronger customer retention strategies       |
| Review     | Delivery delay is a key factor that directly lowers review scores              |
| Time       | Logistics resources should be allocated early in the week (especially Tuesday) |
| Region     | Optimize São Paulo-centered logistics hubs and monitor delay-prone routes      |
| Prediction | Product category, price, and seller/customer location are key predictors       |

<br />

## 👥 Team

- Hong Gil-dong (@username1)
- Kim Cheol-su (@username2)
