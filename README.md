# 🍔 Food Delivery Data Analysis using SQL

## 📌 Project Overview
This project analyzes a food delivery dataset (50,000+ records) to uncover customer behavior, revenue patterns, and business insights.

The goal is to simulate real-world business analysis using SQL.

## 📊 Dataset Details
- Total Records: 50,000+
- Columns: 19
- Features include:
  - City, Cuisine, Meal Type
  - Order Value, Delivery Fee
  - Mood, Hunger Level
  - Weather Conditions
  - Customer Type (Repeat/New)

## ❓ Business Questions Solved

1. Which city generates the highest revenue?
2. Which cuisine is most profitable?
3. Do repeat customers spend more?
4. Does rainy weather increase orders?
5. How delivery time affects ratings?
6. What is the peak ordering time?
7. Do mood and hunger affect spending?

## 🔍 Key Insights

- 💰 Repeat customers contribute significantly higher revenue
- 🌧 Orders increase during rainy weather
- ⏱ Faster delivery leads to better ratings
- 🍜 Certain cuisines dominate in specific cities
- 🧠 Customers with high hunger levels spend more

## 🛠 SQL Skills Used

- GROUP BY & Aggregations
- CASE WHEN
- Window Functions (RANK, OVER)
- CTE (WITH clause)
- Data Segmentation

## 💡 Sample Query
<img width="640" height="194" alt="image" src="https://github.com/user-attachments/assets/abb94db0-1d2e-47f1-808b-5a79521e75e8" />

```sql
SELECT 
    city,
    SUM(order_value) AS revenue
FROM food_ordering_behaviour
GROUP BY city
ORDER BY revenue DESC;

## 📈 Conclusion
- Repeat customers generate higher revenue
- Rain increases order volume
- Fast delivery leads to better ratings



