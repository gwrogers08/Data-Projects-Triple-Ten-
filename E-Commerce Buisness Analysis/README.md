# 🛒 E-Commerce Business Analysis

## 📌 Project Overview
**explore user activity data** to uncover insights about customer behavior, conversion rates, and retention trends. The dataset captures each step in a customer’s journey — from viewing a product to making a purchase.

---

## 📂 Dataset Description
The raw dataset consists of user interaction logs with the following fields:

- **user_id** → Unique customer IDs  
- **event_type** → Activity type (view, add to cart, purchase)  
- **category_code** → Product category viewed or purchased  
- **brand** → Product brand  
- **price** → Price of the product (USD)  
- **event_date** → Date of activity (YYYY-MM-DD)

---

## 📊 Analysis Performed
Using the transaction logs, several key analyses were conducted:

### 🔹 Conversion Funnel
- **10,453** users viewed product pages  
- **29.04%** added an item to their cart  
- **35.61%** of those who added to cart completed a purchase  
- Final **conversion rate: 10.34%**

### 🔹 Cohort & Retention Analysis
- Customers were grouped by **month of first purchase**  
- Retention tracked over **four months post-purchase**  
- Findings:  
  - **Sept 2020** showed the highest retention at 12.5% after 1 month  
  - By **Feb 2021**, no retained customers remained active  
  - Overall trend: retention declined steadily across cohorts

### 🔹 Key Insights
- Strong initial engagement but significant **drop-off after first purchase**  
- Customers acquired in late 2020 had **weaker retention** than earlier cohorts  
- The **conversion funnel bottleneck** lies between product views and cart additions

---

## 📑 Project Deliverables
- **Executive Summary** → High-level findings and recommendations  
- **Conversion Funnel Analysis** → User flow from product view → purchase  
- **Cohort Retention Analysis** → Month-over-month customer retention  
- **Raw User Activity Exploration** → Cleaned and structured logs for insights  

---

## 🛠️ Tools & Skills
- **Data Cleaning & Analysis** → Google Sheets, Excel functions  
- **Cohort & Retention Calculations** → Pivot tables, formulas  
- **Data Visualization** → Conversion funnel & retention charts  
- **Business Insights** → Translating raw logs into actionable recommendations  

---

## 📈 Results Snapshot
| Event Type      | Unique Users | Conversion Rate | Next Stage Conversion |
|-----------------|--------------|-----------------|------------------------|
| View            | 10,453       | 100%            | –                      |
| Add to Cart     | 3,036        | 29.04%          | 29.04%                 |
| Purchase        | 1,081        | 10.34%          | 35.61%                 |

---

## 📘 Key Takeaways
- Optimize **product page experience** to improve cart additions.  
- Implement **retention strategies** (loyalty programs, email campaigns) to sustain repeat purchases.  
- Focus on **long-term customer engagement**, not just acquisition.  

