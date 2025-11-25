# **TELECOM CUSTOMER CHURN ANALYSIS – END TO END PROJECT
*(SQL → Python → Power BI)*
---

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

The data consists of 7,043 customer records with 21 features, stored in a local MySQL database.
Target Variable: Churn (Yes/No)
Data Split: 73.4% Retained, 26.6% Churned.
**Key Features**:
Demographics: Gender, SeniorCitizen, Partner, Dependents.
Services: Phone, MultipleLines, Internet (DSL/Fiber), Security, Backup.
Account Info: Tenure, Contract, PaymentMethod, MonthlyCharges.

---

## **Data Engineering & Workflow**

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

## **Key Insights & Findings**

- **Churn Rate:** 26.6% (industry benchmark: 10–15%)  
- **Churn Drivers:**  
  - Short tenure (<12 months)
  - High monthly charges
  - Month-to-month contracts
  - No tech support, electronic check payment
- **Modeling:**  
  - High-risk group (>0.7 churn probability): ~6% of all customers, high-priority for retention
  - Model evaluated on accuracy, ROC-AUC, and business interpretability

---

## **Business Recommendations**

| Challenge                    | Action                                       |
|------------------------------|----------------------------------------------|
| New customers churn quickly  | Improve onboarding; early support contacts   |
| High monthly charges         | Personalized discounts, plan bundling        |
| Flexible contracts           | Upsell annual/semi-annual plans; loyalty offers |
| Lack of tech support         | Free/basic support included                  |
| Electronic check payers      | Incentivize transition to auto-pay           |
| Fiber optic churn            | Service/price benchmarking & outreach        |

Estimated **monthly revenue saved:** ₹20 lakhs+.  
**Annual saving potential:** ₹2.4–3 crore with targeted retention.

---

## **Conclusion**

This project successfully demonstrates how data analytics can translate into tangible business value. By moving from reactive analysis to predictive modeling, the company can reduce its churn rate from ~26% down towards the industry average, saving millions in annual revenue while improving customer satisfaction.

---

## **Tools & Technologies Used**

- **SQL / MySQL:** Data storage and retrieval  
- **Python:** Data extraction, cleaning, EDA, feature engineering, modeling (Pandas, NumPy, Scikit-learn)  
- **Power BI:** Business dashboarding and interactive visualization  
- **Jupyter Notebook / IPython:** Code, documentation, and workflow presentation  
---



---

**Author:** [Priyanka Lakra]  
