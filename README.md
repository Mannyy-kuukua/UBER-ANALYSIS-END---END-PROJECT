# UBER-ANALYSIS-END-END-PROJECT
END TO END DATA ANALYSIS DUMMY PROJECT



# 🚖 Uber Trip Analysis – June 2024


## 📌 Project Overview

This project analyzes Uber rides recorded in **June 2024** with the goal of identifying trip trends, customer behavior, and revenue drivers. Using **MySQL, Python, and Power BI**, the workflow spans from raw data storage and cleaning to visualization and actionable insights.

---

## 🛠️ Tools & Technologies

* **MySQL Workbench** – Database storage & management
* **Python** – Exploratory Data Analysis (EDA)

  * `pandas`, `numpy` for data manipulation
  * `matplotlib`, `seaborn` for visualizations
* **Power BI** – Dashboard and interactive reporting

---

## 📂 Project Structure

```
├── Uber Dataset.csv        # Raw dataset  
├── Trip Analysis.csv        # Cleaned dataset  
├── Location.csv             # Trip location data  
├── Loc-Merged.csv           # Merged trips + location dataset  
├── scripts/                 # Python EDA scripts  
│   └── eda.ipynb  
└── dashboard/               # Power BI dashboard file (.pbix)  
```

---

## 🔎 Analysis Workflow

### 1. Database Setup (MySQL)

* Created Uber database
* Imported CSV files using **Import Wizard**
* Duplicated tables for backup & best practice

### 2. Python-MySQL Connection

```python
import pandas as pd
import mysql.connector

connection = mysql.connector.connect(
    host="localhost",
    user="root",
    password="yourpassword",
    database="uber"
)

query = "SELECT * FROM trips"
df = pd.read_sql(query, connection)
print(df.head())
```

### 3. Data Cleaning & Feature Engineering

* Checked for missing values, duplicates, and inconsistent entries
* Created new columns:

  * **Total Revenue**
  * **Trip Duration**
  * **Calendar Features** (day of week, week number, trip hour)

### 4. Visualizations (Python)

* **Line & Bar Charts** – Revenue and trip trends
* **Pie Charts** – Payment methods & vehicle types
* **Histograms** – Distribution of trips

### 5. Exporting Cleaned Data

* Saved as `Trip Analysis.csv` for Power BI

---

## 📊 Dashboard Insights (Power BI)

Key metrics and trends:

* **Total Trips:** 103,728
* **Total Revenue:** \$1.55M
* **Distance Covered:** \~348,900 miles
* **Busiest Day:** Sundays
* **Least Busy Day:** Fridays
* **Payment Method Preference:** Uber Pay (67%)
* **Top Pickup Locations:** Brooklyn, Manhattan, Queens
* **Most Ordered Vehicle:** UberX (37.58%)
* **Peak Hours:** 6 AM – 5 PM

---

## 📌 Insights

* 🚗 Ride volume grows steadily during the week, peaking on Sundays
* 💰 UberX dominates demand, while Uber Pay is the top payment method
* 🗺️ Brooklyn, Manhattan, and Queens generate the highest demand

---

## 💡 Recommendations

* 📉 **Boost Friday usage:** Discounts, referral bonuses, or ride bundles
* 🤝 **Corporate partnerships:** Subsidized weekday rides for employees
* 🌱 **Expand Uber Green:** Attract eco-conscious riders with comfort upgrades
* 📲 **Feedback Integration:** Use in-app surveys for continuous service improvement

---

<img width="1569" height="863" alt="Uber" src="https://github.com/user-attachments/assets/0ad3d26f-3e49-411c-b42a-b2958e580ca2" />


<img width="1125" height="672" alt="hourly" src="https://github.com/user-attachments/assets/6ebe45a6-7db3-45f8-a443-085d879345b3" />

  


---<img width="1841" height="817" alt="p1" src="https://github.com/user-attachments/assets/54ea225c-49f0-4817-9970-f0bf2519405a" />


## 🚀 Conclusion

This project demonstrates how combining **SQL, Python, and Power BI** creates a full **data analysis pipeline** from raw data to insights. The findings highlight patterns in customer behavior and provide recommendations for **data-driven business decisions**.

---

✨ *Author: \[Manasia Dankwah Sackey]*
📧 Contact: \[(email:sackeymanasia@gmail.com)]
🔗 [LinkedIn](www.linkedin.com/in/manasia-sackey | [Portfolio](github.com/Mannyy-kuukua)


