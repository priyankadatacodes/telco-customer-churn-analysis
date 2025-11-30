#  **TELECOM CUSTOMER CHURN ANALYSIS – END TO END PROJECT
![SQL](https://img.shields.io/badge/SQL-MySQL-orange) →![Python](https://img.shields.io/badge/Python-3.10%2B-blue)→![Power BI](https://img.shields.io/badge/BI-Power%20BI-yellow)

---
![Telecom Churn Analysis](https://raw.githubusercontent.com/priyankadatacodes/telco-customer-churn-analysis/blob/main/telecom_churn_analysis.png)

## **Project Overview**

This project focuses on identifying risk factors associated with customer churn in the telecommunications industry. By leveraging MySQL for data management and Python for predictive modeling, we analyzed customer behavior to build a machine learning solution that flags high-risk users. The project further extends into a Power BI dashboard for real-time monitoring and quantifies the financial impact of retention strategies.

---

## **Problem Statement**

Customer churn is a critical and costly problem in subscription businesses. Here, the telco company faces a **churn rate above 26%**—putting future revenue at risk.  
**Key Questions:**
- What factors drive customer churn most?
- Which customers are at highest risk?
- How can the business focus its retention efforts for maximum ROI?

---

## **Dataset Summary**

- The data consists of 7,043 customer records with 21 features, stored in a local MySQL database.
- Target Variable: Churn (Yes/No)
- Data Split: 73.4% Retained, 26.6% Churned.
**Key Features**:
- Demographics: Gender, SeniorCitizen, Partner, Dependents.
- Services: Phone, MultipleLines, Internet (DSL/Fiber), Security, Backup.
- Account Info: Tenure, Contract, PaymentMethod, MonthlyCharges.

---

## **Approach**

![Telecom Churn Analysis Worklflow](https://raw.githubusercontent.com/priyankadatacodes/telco-customer-churn-analysis/blob/main/churn_workflow.png)

> **1. Data Ingestion:**  
  - Downloaded raw customer churn dataset from Kaggle  
  - Created relational table in **MySQL** (well-defined schema with correct data types)
  - Imported data to MySQL for storage, retrieval, and data integrity

> **2. Data Extraction & Cleaning (Python):**  
  - Used **Python (Pandas + SQLAlchemy)** to fetch data directly from the MySQL database  
  - Performed exploratory data analysis (EDA), cleaned missing values, corrected data types  
  - Feature engineering: tenure groups, categoricals, numeric conversions  
  - Saved the cleaned, analysis-ready dataset for next steps

> **3. Analysis & Modeling:**  
  - Conducted descriptive analytics, churn drivers analysis, group statistics  
  - Built predictive models (Logistic Regression, Random Forest) to classify high-risk customers  
  - Evaluated model performance, calculated churn probabilities

> **4. Business Dashboarding (Power BI):**  
  - Imported cleaned dataset to Power BI  
  - Created interactive dashboards:  
    - Churn summary, key KPIs, feature drilldowns, filterable segments
    - Model prediction visualization and high-value customer lists

> **5. Reporting & Delivery:**  
  - Documented all steps and business logic in this README for clarity and review

---

## **Tools & Technologies Used**

- **SQL / MySQL:** Data storage and retrieval  
- **Python:** Data extraction, cleaning, EDA, feature engineering, modeling (Pandas, NumPy, Scikit-learn)  
- **Power BI:** Business dashboarding and interactive visualization  
- **Jupyter Notebook / IPython:** Code, documentation, and workflow presentation

---
## **Key Outcomes of the Analysis**

- **Churn Rate:** 26.58%
- **Retained Customers:** 73.42%
- **High-Risk Customers Identified:** 6.33%
- **Top Churn Drivers:** Low tenure, high monthly charges, digital billing

These results help identify areas where the company can apply targeted retention efforts.

---

## **Insights Summary**

### 1. Overall Customer Situation

The company is experiencing a 26.58% churn rate, which means one in every four customers is leaving. While 73.42% of customers are retained, even a small reduction in churn could make a significant difference in revenue and customer satisfaction.

### 2. Customer Demographics

- The gender ratio is balanced, with no strong churn bias by gender.
- Only 16% of customers are senior citizens; this is not a major segment for churn.
- Customers who have partners or dependents are slightly more stable and less likely to churn.

### 3. Tenure: Main Indicator of Churn

- Median tenure for retained customers is 38 months.
- Median tenure for churned customers is just 10 months.
- This shows that new customers (under one year) are much more likely to leave, which may highlight issues with onboarding or initial experience.

### 4. Billing and Service Behavior

- 90% of customers use phone service, so this feature does not strongly influence churn.
- Paperless billing is linked to stronger churn, possibly due to dissatisfaction with digital billing or unclear charges.
- Median monthly charges are ₹64.5 for retained and ₹79.7 for churned customers, suggesting customers paying higher bills may feel less value for money.

### 5. Revenue Impact

- Retained customers have a median total lifetime charge of ₹1683.6.
- Churned customers only contribute a median of ₹703.5 before leaving, which shows the business is losing customers early and reducing lifetime value.

### 6. Top Churn Drivers

| Feature           | Correlation with Churn |
|-------------------|----------------------|
| Churn Probability | 0.557                |
| Tenure            | 0.354                |
| TotalCharges      | 0.199                |
| MonthlyCharges    | 0.193                |
| PaperlessBilling  | 0.191                |

Customers with low tenure and high bills are at the highest risk of churning.

### 7. Model-Based Churn Risk

- Average predicted churn probability is 0.27
- High-risk group (churn probability above 0.7) is 6.33% of all customers
- This group should be the main focus for retention campaigns

---

## Practical Recommendations

1. **Improve Onboarding for New Customers:**  
   Since newer customers are more likely to churn, a more structured onboarding process and early customer support may help increase retention.

2. **Address High Billing Concerns:**  
   Customers with higher monthly charges leave more frequently. Review billing policies, consider targeted discounts, or bundle offers for those paying more.

3. **Clarify or Enhance Digital Billing:**  
   Paperless billing is associated with higher churn. Make digital statements clearer or offer optional paper statements to increase transparency.

4. **Focus Retention on High-Risk Segment:**  
   Use model predictions to identify and proactively engage the 6% of customers with the highest churn risk, through personalized offers or support.

5. **Encourage Long-term Contracts:**  
   Since flexible, month-to-month plans are linked to higher churn, incentivize annual or longer contracts where appropriate.

6. **Offer Basic Tech Support:**  
   Providing complimentary support packages can help reduce attrition, especially for new or high-value customers.

7. **Monitor Customer Lifetime Value:**  
   Make efforts to increase the LTV of at-risk customers, especially in the first year.

*All recommendations are based on the findings from the data analysis. As a fresher, I focused on actionable insights that can be realistically implemented by a telecom business and demonstrated my understanding of analytics-driven decision making.*

---

## **Conclusion**

This project successfully demonstrates how data analytics can translate into tangible business value. By moving from reactive analysis to predictive modeling, the company can reduce its churn rate from ~26% down towards the industry average, saving millions in annual revenue while improving customer satisfaction.

---

**Author:** [Priyanka Lakra]  
