📊 Customer Churn Retention Analysis
🏢 Project Overview

This Power BI project analyzes customer churn and retention patterns to help business decision-makers understand why customers leave and identify opportunities to improve retention.
The dashboard provides a 360° view of customer demographics, subscription contracts, internet services, and support interactions to uncover key churn drivers.

🎯 Business Requirement
The management team wants to identify the factors contributing to customer churn and build strategies to improve customer loyalty.

The objectives of this project are:
Measure and monitor customer churn rate.
Identify high-risk customers and segments prone to churn.
Analyze contract type, payment method, and internet service impact on churn.
Provide actionable insights and recommendations for retention improvement.

🧾 Dataset Details
File: 02 Churn-Dataset.xlsx
Records: 7,043 customers
Columns: 23 attributes including:
Demographics: Gender, Senior Citizen, Partner, Dependents
Account Info: Tenure, Contract, Payment Method, Monthly/Total Charges
Services: Internet, Online Security, Backup, Device Protection, Tech Support, Streaming TV/Movies
Support: Admin and Tech Tickets
Churn: Whether a customer has left (Yes/No)

⚙️ Data Preparation
Performed in Power Query Editor (Power BI Desktop)
Cleaned and standardized columns (Yes/No, binary flags).
Created a calculated column Loyalty to categorize customers by tenure (<1 Year, <2 Years, … <6 Years).
Removed redundant fields and ensured correct data types.
Validated against missing and inconsistent records.

📐 Data Modeling
Built a single fact table (Customer Churn) with derived measures.
Created key DAX Measures:
Churn Rate % = DIVIDE(COUNTROWS(FILTER('Customer Churn', [Churn] = "Yes")), COUNTROWS('Customer Churn'))
Average Monthly Charges
Average Total Charges
Admin Tickets, Tech Tickets, and Service Usage %

📊 Dashboard Design
The Power BI report contains three interactive pages:

1️⃣ Customer Churn Overview
Total Customers, Churn Rate, and Revenue KPIs
Churn by Tenure, Contract Type, Payment Method, and Internet Service
Demographic Distribution (Gender, Senior Citizen, Dependents)

2️⃣ Customer Risk Dashboard
Customer churn vs Internet Service
Churn rate comparison by Contract Type
Monthly Charges vs Churn Trends
Admin and Tech Support Tickets analysis

3️⃣ Service Insights Dashboard
Comparison of churn across service features (Online Security, Tech Support, Streaming Services, Device Protection)
Identifies service combinations leading to higher churn

💡 Key Insights
27% churn rate among total 7,043 customers.
Customers on Month-to-Month contracts have the highest churn.
Customers without Online Security, Tech Support, or Phone Service are more likely to leave.
Fiber Optic customers (42%) showed the highest churn rate compared to DSL or No Internet Service.
$16.06M in yearly revenue and $456.1K in monthly charges at risk.
Customers with higher tenure and longer contracts (1–2 years) show better retention.

🧠 Recommendations
Encourage customers to shift from Month-to-Month to Annual or Two-Year Contracts through discounts or loyalty programs.
Educate customers on benefits of Online Security and Tech Support services.
Improve Fiber Optic Service Quality and resolve technical complaints faster.
Introduce targeted retention campaigns for new customers in the first 12 months.
Aim to increase long-term contracts and automatic payment adoption by 5% annually.

🛠 Tools & Technologies
Power BI Desktop – Dashboard design & data modeling
Power Query Editor – Data transformation
Microsoft Excel – Data source
DAX (Data Analysis Expressions) – KPI calculations

📎 Files Included
File Name	Description
Customer Churn Retention.pbix	Power BI Report File
02 Churn-Dataset.xlsx	Source data file
Customer Churn Retention.pdf	Dashboard snapshot (exported PDF)

👨‍💻 Author
Kalpesh Nardekar
Business Intelligence Developer | Power BI | Data Analytics
📧 Email: [kalpeshnardekar@outlook.com]
