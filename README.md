# 💳 Bank Loan Analysis Project

This project uses **Python (EDA)** and **Power BI** to analyze a bank’s loan portfolio and answer key business questions such as:

- Which states, terms and customer segments bring the highest funded amounts?
- How are **loan applications, funded amounts, and repayments** trending over time?
- What customer profiles (employment, house ownership, purpose) are most strongly associated with higher funding?

---

## 🛠 Tech Stack

- **Python** – Data cleaning & exploratory data analysis  
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
- **Power BI** – Data modelling, DAX measures & interactive dashboards  
- **Excel** – Source data files

---

## 📂 Project Structure

- `notebooks/loan_eda.ipynb` – Python notebook for data cleaning and EDA  
- `data/` – Raw and cleaned datasets  
- `dashboard/Bank_Loan_Analysis.pbix` – Power BI report  
- `images/` – Exported dashboard screenshots  

Example images used in this README:

![Bank Loan Dashboard – Overview](https://github.com/DinakarShetty/Bank-Loan-Analysis-Project/blob/main/Bank%20Loan%20Analysis%201.jpg)
![Bank Loan Dashboard – Segment Analysis](https://github.com/DinakarShetty/Bank-Loan-Analysis-Project/blob/main/Bank%20Loan%20Analysis%202.jpg)

---

## 🔍 EDA Highlights (Python)

Using Python, the dataset was explored and prepared with steps such as:

- Handling missing values and inconsistent categories  
- Converting date columns and deriving **month** and **year** for trend analysis  
- Creating new features such as:
  - Loan term buckets (36 vs 60 months)
  - High-value vs low-value funded amounts
- Generating summary statistics and visualizations to understand:
  - Distribution of funded amounts and received amounts  
  - Relationship between **loan purpose**, **employment length**, **house ownership**, and funded value  
  - State-wise funding patterns and concentration

The cleaned dataset was then exported and used as the data source for the Power BI model.

---

## 📊 Power BI Dashboard Summary

### 1️⃣ Portfolio Overview

- **Total funded amount by state** clearly shows **CA, NY and TX** as the top-performing states, with **California alone contributing ~78M+** in funded loans.  
- **Monthly trends** indicate consistent growth:
  - **Loan applications** rise steadily from ~2.3K in January to ~4.3K in December.  
  - **Total funded amount** increases from ~25M to ~54M across the year.  
  - **Total received amount** also follows an upward trend, ending near **58M** in December.

### 2️⃣ Loan Term & House Ownership

- Funding is dominated by **36-month loans (~63%)**, compared to **60-month loans (~37%)**, suggesting a preference for shorter-term products.  
- By house ownership:
  - **Mortgage customers (~219M)** account for the largest share of funded amount.  
  - **Renters (~186M)** form the next major segment.  
  - **Fully owned houses (~30M)** represent a smaller but important group.

### 3️⃣ Employment & Loan Purpose

- Customers with **10+ years of employment** contribute the highest funded amount, around **116M**, indicating that **stable employment** is strongly associated with higher loan approvals.  
- **Debt consolidation** is the dominant loan purpose with **~232.5M** funded, followed by:
  - **Credit card (~58.9M)**  
  - **Home improvement (~33.4M)**  
  - Other purposes (small business, major purchase, car, medical, etc.) at lower but meaningful volumes.

---

## 🎯 Key Business Insights

- Growth in both **applications and funding** month-on-month shows strong demand and room for targeted campaigns in peak months.  
- **Short-term (36-month) loans, mortgage & renter segments, and long-tenured employees** form the core of the loan portfolio and should be prioritized for cross-sell and retention strategies.  
- The dominance of **debt consolidation and credit card loans** suggests an opportunity to design specialized products and risk models tailored to these use cases.  
- State-wise analysis highlights **high-value regions (e.g., CA, NY, TX)** where focused marketing and relationship management can generate additional growth.

