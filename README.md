# 📊 Customer Churn Analysis (SQL, Python & Power BI)

## 🔹 Project Overview

Customer churn is one of the biggest challenges for subscription-based businesses. This project analyzes customer churn patterns using **SQL, Python, and Power BI** to identify the key reasons why customers leave and provide actionable insights to reduce churn.

The project is designed as an **end-to-end pipeline** — from raw CSV data to a cleaned SQL database, exploratory analysis in Python, and finally an interactive Power BI dashboard for storytelling.

---

## 🔹 Project Goals

* Import and clean customer churn data using **PostgreSQL**.
* Perform **Exploratory Data Analysis (EDA)** in Python to uncover churn drivers.
* Build an interactive **Power BI dashboard** to visualize churn KPIs and trends.
* Deliver **business insights & recommendations** to reduce churn.

---

## 🔹 Workflow

### 1. Database Creation & Cleaning (SQL)

* Loaded raw CSV into **PostgreSQL**.
* Created `churn` table with all customer attributes.
* Performed initial exploration:

  * % of Gender distribution
  * Types of Contracts and their percentage
  * Payment Method distribution
  * Top 5 Churn Reasons
* Checked and handled null values using `COALESCE`.
* Created a cleaned final table `churn_final` ready for analysis【93†SQL Queries.sql】.

### 2. Exploratory Data Analysis (Python)

Performed detailed EDA in **Jupyter Notebook** (`EDA.ipynb`) covering:

* **Univariate Analysis**: Distribution of churn, tenure, charges.
* **Bivariate Analysis**: Crosstabs of churn with contract type, payment method, internet type, and service features.
* **Key Findings**:

  * Most churned customers were on **Month-to-Month contracts**, while One-Year and Two-Year contracts showed much lower churn.
  * **Bank Withdrawal users churned the most (34%)**, while Credit Card users churned less (15%).
  * Customers paying the **highest monthly charges** churned the most.
  * Customers without **Online Security, Online Backup, Device Protection, or Customer Support** had churn rates of \~29–32%.

### 3. Dashboard Building (Power BI)

Connected Power BI directly to the PostgreSQL database (`churn_final` table) and built an **interactive churn dashboard** (`Churn Dashboard.pbix`).

Dashboard features:

* **KPI Cards**: Total Customers, Churn Rate, Retained Customers.
* **Bar/Column Charts**: Churn by contract type, payment method, internet type.
* **Map**: Customers by state.
* **Trend Chart**: Churn by tenure group.
* **Stacked Bars**: Service features (Online Security, Backup, Support) vs churn.

### 4. Documentation

* Prepared this README as a structured project report.
* Contains workflow, tech stack, key insights, and recommendations.

---

## 🔹 Tech Stack

* **SQL (PostgreSQL)** → Database creation, data cleaning, initial exploration.
* **Python (Pandas, Matplotlib, Seaborn)** → EDA & churn driver analysis.
* **Power BI** → Interactive dashboard and business storytelling.

---

## 🔹 Key Insights

* **Contract Type**: Month-to-Month contracts have the highest churn, while long-term contracts reduce churn significantly.
* **Payment Method**: Bank Withdrawal customers churn more; Credit Card users are more loyal.
* **Monthly Charges**: Higher charges correlate with higher churn.
* **Services**: Lack of Online Security, Backup, Device Protection, or Support strongly contributes to churn (\~29–32%).
* **Tenure**: New customers (low tenure) are more likely to churn compared to long-tenure customers.

---

## 🔹 Business Recommendations

* Offer **discounts and incentives** to encourage Month-to-Month customers to switch to longer contracts.
* Promote **credit card / auto-pay options** to reduce churn.
* Provide **bundled service offers** (Online Security, Backup, Device Protection) to improve retention.
* Focus on **early customer experience** to reduce churn in the first few months.

---

## 🔹 How to Run This Project

1. Clone the repo:

   ```bash
   git clone https://github.com/your-username/Customer-Churn-Analysis-SQL-Python-PowerBI.git
   ```
2. Load the SQL scripts (`SQL Queries.sql`) into PostgreSQL to create and clean the database.
3. Run the Python notebook (`EDA.ipynb`) for churn EDA.
4. Open the Power BI file (`Churn Dashboard.pbix`) and connect it to your SQL database.

---

## 🔹 Dashboard Preview

*(Insert screenshot of your Power BI dashboard here)*

---

## 📌 Author

Your Name — *Aspiring Data Analyst*
