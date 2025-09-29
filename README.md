<div style="font-family:'Times New Roman', serif; font-size:10px;">
  
# 🍕Pizza Sales - Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project analyzes a year’s worth of pizza sales data from a fictitious pizza place.  
The dataset includes order information, pizza details, and ingredients.  
The analysis provides insights into **revenue trends, customer purchasing behavior, and pizza performance**.

The project demonstrates how to:
- Clean and merge multiple CSV files into one dataset  
- Perform exploratory data analysis (EDA) with **Pandas** and **Matplotlib**  
- Generate business insights such as **top-selling pizzas, peak sales hours, and underperforming items**

---

## 📂 Dataset Description
The analysis uses four CSV files:

| File Name          | Description                                                        |
|--------------------|--------------------------------------------------------------------|
| `orders.csv`       | Contains order IDs and timestamps                                  |
| `order_details.csv`| Holds details of each pizza in an order (pizza ID, quantity, etc.) |
| `pizzas.csv`       | Includes pizza IDs, size, and price                                |
| `pizza_types.csv`  | Provides pizza names, categories, and ingredients                  |

After merging, the final dataset has **48,620 rows × 12 columns**, with the following fields:

| Column            | Description                                |
|-------------------|--------------------------------------------|
| order_details_id  | Unique row identifier                      |
| order_id          | Unique order identifier                    |
| pizza_id          | Pizza + size identifier (e.g., `hawaiian_m`) |
| quantity          | Number of pizzas ordered                   |
| date              | Date of order                              |
| time              | Time of order                              |
| pizza_type_id     | Base pizza type (e.g., `hawaiian`)         |
| size              | Pizza size (S, M, L, XL, XXL)              |
| price             | Price of the pizza                         |
| name              | Full pizza name (e.g., The Hawaiian Pizza) |
| category          | Pizza category (Classic, Supreme, Veggie, etc.) |
| ingredients       | List of pizza ingredients                  |
| revenue           | Calculated as `price × quantity`           |

---

## 🔧 Data Preparation
- Loaded and merged all 4 CSV files into a single DataFrame  
- Checked for missing values (none found)  
- Created additional features such as:  
  - `revenue = price × quantity`  
  - `hour` (from time)  
  - `day_of_week` (from date)  
  - `month` (from date)  

---

## 📊 Key Business Insights

### 💰 Total Sales & Orders
- **Total Revenue:** $817,860.05  
- **Total Quantity Sold:** 49,574 pizzas  
- **Total Orders:** 21,350  
- **Number of Pizza Types:** 32  
- **Average Pizza Price:** $16.49  

---

### ⏰ Sales by Time
- **Peak Sales Hour:** 12:00 PM (lunch time)  

### 📅 Sales by Day
- **Best Day for Sales:** Friday ($136,073.90 revenue)  
- **Lowest Sales Day:** Sunday ($99,203.50 revenue)  

### 📆 Sales by Month
- **Best Month:** July ($72,557.90 revenue)  
- **Notable dips:** February & October  

---

### 🍕 Top 5 Bestselling Pizzas
1. The Classic Deluxe Pizza (2,453 sold)  
2. The Barbecue Chicken Pizza (2,432)  
3. The Hawaiian Pizza (2,422)  
4. The Pepperoni Pizza (2,418)  
5. The Thai Chicken Pizza (2,371)  

➡️ **Best Seller:** *The Classic Deluxe Pizza* 🎉  

---

### 🥴 Underperforming Pizzas
- **Least Popular Pizza:** The Brie Carre Pizza (490 sold)  
- Other weak performers: Mediterranean, Calabrese, Spinach Supreme, Soppressata  

---

## 📊 Visualizations
The project includes clear **Matplotlib-based visualizations**:
- Sales by hour of the day  
- Sales by day of the week  
- Sales by month (bar & line charts)  
- Top 5 bestselling pizzas  
- Bottom 5 least-selling pizzas  

---

## 🚀 Tools & Libraries Used
- Python 3.10+  
- **Pandas** – Data cleaning & manipulation  
- **Matplotlib** – Visualization  
- **Jupyter Notebook** – Development environment  

---

## 📈 Business Takeaways
- Fridays at lunchtime are the most profitable period  
- July is peak season, suggesting higher demand mid-year  
- Classic pizzas dominate sales, while premium/unique pizzas underperform  
- Streamlining or promoting weak pizzas may improve profitability  

---

## 📓 Notebook
🔗 [**PHILIPA OPOKU.ipynb**](https://github.com/philipaopoku-ds/Pizza-Sales-_Exploratory-Data-Analysis/blob/main/PHILIPA%20OPOKU.ipynb) – Full Jupyter notebook with the code, data merging, visualizations, and analysis.

---
</div>
