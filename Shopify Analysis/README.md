# Shopify App Analysis (Power BI)

## 📊 Project Overview
This project analyzes the **landscape of apps on the Shopify platform** using data scraped from publicly available Shopify websites. The goal is to identify key factors that contribute to the success of a Shopify app.  

The analysis was built in **Power BI**, with each section of the project presented as a dedicated page in the report. Screenshots of visuals and supporting calculations are included to demonstrate findings and methodology.

---

## 📂 Dataset
The dataset (`shopify.xlsx`) contains 4 tables:

- **apps**: Details of Shopify marketplace apps  
- **apps_categories**: Join table connecting apps to categories  
- **categories**: Categories of apps (each app can have multiple)  
- **reviews**: User reviews, including ratings, comments, and developer replies  

---

## 🔎 Analysis Breakdown

### **Part 1: App Landscape**
- **KPI Card** – Count of unique apps in the dataset  
- **Line Chart** – Review counts over time by `lastmod` date  
- **Scatterplot** – Review count vs. average rating, annotated with insights  

**Key Insight:**  
Most apps fall within **1–5k reviews**, with average ratings clustering between **4–5 stars**:contentReference[oaicite:1]{index=1}.  

---

### **Part 2: Reviews**
- **New Column (DAX)**:  
  - `helpful_reviews = rating * (1 + helpful_count)`  
  - Captures review quality weighted by helpfulness  
- **KPI Card** – Average `helpful_reviews` score (≈ **5.48**)  
- **New Column (DAX)**:  
  - `developer_answered = IF(ISBLANK(developer_reply),0,1)`  
  - Tracks if a developer responded to a review  
- **Scatterplot** – Average rating vs. developer responsiveness  

**Key Insight:**  
Apps with developers who **respond to reviews** tend to maintain **higher average ratings**:contentReference[oaicite:2]{index=2}.  

---

### **Part 3: App Reviews**
- **Relationship**: Connected `Reviews` (app_id) to `Apps` (id) as many-to-one  
- **Bar Chart** – Developer vs. sum of ratings  
- **Adjusted Bar Chart** – Developer vs. average `helpful_reviews` (to account for skew from many low-star ratings)  
- **Bar Chart with Filter** – Developer responsiveness (`developer_answered`), filtered for apps with **>500 reviews**  

**Key Insight:**  
- Developers like **Hexom, Privy, FireApps, and Shopify** show high review engagement.  
- **Transcy Apps, Identixweb, and HulkApps** appear among the **most responsive** developers:contentReference[oaicite:3]{index=3}.  

---

## 🛠 Tools & Skills Used
- **Power BI** (visualization, data modeling, DAX calculations)  
- **Data Cleaning & Transformation** (relationships between tables)  
- **Business Intelligence** (KPI tracking, trend analysis, developer benchmarking)  

---

## 📸 Sample Visuals
Below are sample report outputs (see full PDF for all):  

- Review count trends over time  
- Scatterplot of ratings vs. reviews  
- Developer responsiveness comparison
  
---

## 📈 Key Takeaways
- The **number of reviews** is not always indicative of app quality — many high-volume apps have mixed ratings.  
- **Developer engagement** (replying to reviews) is strongly correlated with higher user satisfaction.  
- Weighted metrics like **helpful_reviews** give a more accurate picture of true app performance.  
