# Customer Churn Analysis – ABC Communications Ltd

Project Overview

This project was completed as part of the AnalystLab Africa Data Analytics Internship Programme – Week 1.

The objective of this business analytics case study is to investigate customer churn at ABC Communications Ltd, identify customer segments and behaviours associated with higher churn, and provide actionable recommendations to improve customer retention.

The analysis uses the Telco Customer Churn dataset and combines data cleaning, exploratory data analysis, statistical analysis and business-focused visualisation.

Business Questions

The analysis aims to answer the following questions:

1. What does the customer base look like?
2. Which customer segments have the highest churn?
3. Does contract type influence retention?
4. Does tenure affect customer loyalty?
5. Which services are associated with higher churn?
6. Which payment methods have higher churn?
7. What actions should management take?

Dataset

The project uses the Telco Customer Churn Dataset, containing customer demographic information, tenure, subscribed services, contract information, payment methods and billing information.

The dataset contains 7,043 customer records and 21 variables.

Key variables include:

- "customerID" – Unique customer identifier
- "gender" – Customer gender
- "SeniorCitizen" – Senior citizen indicator
- "Partner" – Whether the customer has a partner
- "Dependents" – Whether the customer has dependents
- "tenure" – Number of months the customer has been with the company
- "PhoneService" – Phone service subscription
- "MultipleLines" – Multiple-line subscription
- "InternetService" – Internet service type
- "OnlineSecurity" – Online security subscription
- "OnlineBackup" – Online backup subscription
- "DeviceProtection" – Device protection subscription
- "TechSupport" – Technical support subscription
- "StreamingTV" – Streaming TV subscription
- "StreamingMovies" – Streaming movies subscription
- "Contract" – Contract type
- "PaperlessBilling" – Paperless billing status
- "PaymentMethod" – Payment method
- "MonthlyCharges" – Monthly customer charges
- "TotalCharges" – Total customer charges
- "Churn" – Whether the customer left the company

Data Cleaning & Inspection

The dataset was inspected using Python and JupyterLab.

The following checks were performed:

- Dataset structure and dimensions
- Data types
- Missing values
- Duplicate records
- Unique categorical values
- Whitespace and hidden missing values
- Numerical variables and summary statistics

Cleaning performed

"TotalCharges" was initially stored as an object/text variable instead of a numerical variable.

During inspection, 11 whitespace-only values were identified in "TotalCharges". These values became "NaN" when the column was converted to numeric.

Further investigation showed that these customers had a tenure of 0 months, so their total charges were set to 0 rather than using statistical imputation.

No duplicate records were identified.

Exploratory Data Analysis

The analysis includes:

- Customer distribution by contract type
- Customer distribution by internet service
- Churn rate by contract type
- Churn rate by tenure group
- Churn rate by payment method
- Churn analysis across subscribed services
- Tenure distribution
- Monthly charges distribution
- Monthly charges by churn status using a box plot
- Correlation analysis of numerical variables

The visualisations were created primarily using Python, Pandas, Matplotlib and Seaborn, with Power BI used to create a polished business dashboard.

---

🔍 Key Findings

1. Overall churn

Approximately 1,869 customers churned, compared with approximately 5,174 customers who remained, corresponding to an overall churn rate of approximately 26.5%.

2. Contract type

Month-to-month customers represent approximately 55% of the customer base and have the highest churn rate among the contract categories.

This makes month-to-month customers an important target for retention initiatives.

3. Tenure

Customers in the 0–12 month tenure group have the highest churn rate.

This suggests that the early stage of the customer relationship is a particularly important period for retention.

4. Internet service

Fiber optic customers represent approximately 44% of the customer base and show significantly higher churn than customers in other internet-service categories.

Further investigation is required to determine whether pricing, service quality, customer experience or other factors explain this pattern.

5. Additional services

Customers without Online Security, Online Backup, Device Protection and Tech Support generally show higher churn rates.

These services may therefore be useful indicators when identifying customers at higher risk of churn.

6. Payment method

Customers using electronic check show substantially higher churn than customers using other payment methods.

7. Correlations

The strongest observed numerical relationships include:

- Tenure and TotalCharges: approximately 0.83
- TotalCharges and MonthlyCharges: approximately 0.65
- Tenure and MonthlyCharges: approximately 0.25

These correlations describe relationships between numerical variables and should not be interpreted as proof of causation.

Business Risks

1. High churn among short-tenure customers may result in customers leaving before developing long-term relationships with the company.
2. The large month-to-month customer segment creates a significant group of customers without long-term contractual commitment.
3. High churn within the fiber-optic and electronic-check segments may indicate unresolved pricing, service, billing or customer-experience issues.

Business Opportunities

1. Strengthen customer onboarding and engagement during the first 12 months.
2. Encourage suitable month-to-month customers to transition to longer-term contracts.
3. Increase adoption of relevant security, backup, device-protection and technical-support services while monitoring their effect on retention.

Recommendatione

Based on the analysis, ABC Communications Ltd should:

1. Launch an early-life retention programme targeting customers during their first 12 months.
2. Develop targeted incentives for month-to-month customers to encourage suitable customers to move to longer-term contracts.
3. Investigate high churn among fiber-optic customers by examining pricing, network quality, complaints and onboarding experience.
4. Promote relevant support and protection services and measure whether adoption is associated with improved retention.
5. Review the electronic-check payment journey and encourage reliable alternative payment methods where appropriate.
6. Develop a recurring churn monitoring dashboard to track high-risk customer segments over time.

These recommendations should be validated through further customer feedback and operational data before assuming that any individual service directly causes churn.



Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- JupyterLab
- Power BI
- Microsoft PowerPoint
- Git & GitHub


Project Deliverables

This repository contains the main deliverables for the Week 1 business analytics case study:

- Business Understanding Report
- Dataset Inspection Report
- Jupyter Notebook
- Business Presentation
- Data visualisations
- Cleaned dataset


Author

Cloclo Ndi

Data Analytics Intern – AnalystLab Africa

Skills demonstrated

- Data cleaning
- Exploratory data analysis
- Data visualisation
- Business analysis
- Churn analysis
- Insight generation
- Business recommendations
- Dashboard development
- Data storytelling

Project Contex

This project was completed as part of the AnalystLab Africa Data Analytics Internship Programme – Week 1: Business Analytics Case Study.

The objective of the assignment is to demonstrate the ability to understand a business problem, inspect and analyse a dataset, identify trends and patterns, create professional visualisations, develop business recommendations and present findings professionally.-
