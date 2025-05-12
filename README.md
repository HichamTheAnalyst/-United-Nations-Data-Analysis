# 🌍 United Nations Data Analysis

This project explores and cleans socioeconomic data from the **United Nations** using SQL and Python. It focuses on understanding population distribution, access to basic services, and regional unemployment statistics. The analysis is performed on a **MySQL** database connected via **SQLAlchemy** and visualized in a Jupyter Notebook.

---

## 🧰 Tools & Technologies

- Python (`pandas`, `matplotlib`, `numpy`)
- MySQL (`pymysql`)
- Jupyter Notebook
- `%sql` and `%%sql` magic for SQL execution in Python

---

## 📊 Key Objectives

- Explore data structure (`SHOW COLUMNS`)
- Identify unique records by country and time
- Clean inconsistent country names using string functions
- Handle `NULL` values in unemployment data
- Generate synthetic primary keys using concatenation
- Create a new table: `Geographic_Location`
- Prepare and transform data for further reporting

---

## ✅ Sample SQL Queries

```sql
-- Unique combinations of country, time period, and estimated population
SELECT DISTINCT Country_name, Time_period, Est_population_in_millions
FROM united_nations.Access_to_Basic_Services
LIMIT 5;
