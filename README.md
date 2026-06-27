# DSA3050A Mid-Semester Practical Exam

## Student Information
- **Name:** Geoffrey Chege Mwangi
- **Student ID:** 669566

## Dataset Source
- **URL:** https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling
- **Name:** Churn Modelling Dataset
- **Description:** Real customer data from a European bank, including demographics, account information, and churn status.

## Data Overview
- **Number of Rows:** 10,000
- **Number of Columns:** 14 (original)

## Business Problem
The bank is experiencing increasing customer churn. Management needs a dashboard to identify key drivers of churn and monitor customer retention performance across geography, demographics, and account behaviour.

## Power Query Transformations Performed
1. **Basic Cleaning:** Renamed columns for clarity, changed data types, removed duplicates and blank rows, trimmed text.
2. **Column Management:** Created `Country_Gender` (merge), `HasBalance` (custom), `AgeGroup` (conditional).
3. **Date Handling:** Created `JoinDate` from `Tenure`, extracted Year, Month, Quarter, Day.
4. **Filtering & Sorting:** Filtered rows with CreditScore > 600 and Balance > 0; sorted by CreditScore descending.
5. **Advanced:** Group By (Geography+Gender with multiple aggregations), Pivot (Geography for average CreditScore), Unpivot (CreditScore, Balance, EstimatedSalary), created a parameter (MinCreditScore) for dynamic filtering, and created a Reference Query for summarised churn by geography.

## Dashboard Visuals
- KPI cards (Total Customers, Total Churned, Churn Rate)
- Bar chart (Churn by Geography)
- Column chart (Churn by Gender)
- Line chart (Churn trend by Tenure)
- Donut chart (Churn by ActiveMember)
- Table (customer details)
- Matrix (Avg Balance by Geography and Gender)
- Filled map (Customer distribution by country)
- Scatter plot (CreditScore vs Balance coloured by churn)

## Business Insights
1. Germany has the highest churn rate (32%), suggesting a need for market‑specific retention strategies.
2. Customers with tenure ≤ 2 years churn significantly more than long‑term customers – early engagement is critical.
3. Inactive members have a churn rate 3x higher than active members; reactivation campaigns could improve retention.