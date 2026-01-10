# **Telecom Customer Churn Analysis – End-to-End Project**
![SQL](https://img.shields.io/badge/SQL-MySQL-orange)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Power BI](https://img.shields.io/badge/BI-Power%20BI-yellow)

---

<img src="https://raw.githubusercontent.com/priyankadatacodes/telco-customer-churn-analysis/main/telecom_churn_analysis.png" width="100%">

---

## **Executive Summary**

This project analyzes **customer churn in the telecommunications industry** to identify **high-risk customers**, understand **key churn drivers**, and support **data-driven retention strategies**.

The company is experiencing a **churn rate of ~26.6%**, which poses a serious risk to long-term revenue.  
Using **SQL for data management**, **Python for analysis and predictive modeling**, and **Power BI for reporting**, this project identifies churn patterns and highlights customers most likely to leave.

The outcome enables the business to **prioritize retention efforts**, reduce churn, and protect customer lifetime value.

---

## **Why I Built This Project**

Customer churn is one of the most expensive problems in subscription-based businesses.  
Acquiring new customers costs significantly more than retaining existing ones.

I built this project to:
- Understand **why customers leave**
- Identify **early churn signals**
- Practice combining **descriptive + predictive analytics**
- Translate model outputs into **business actions**

This mirrors a real-world data analyst role where insights must support **revenue and retention decisions**.

---

## **Business Context**

Telecom companies operate on:
- Monthly subscription revenue
- Long-term customer relationships
- High competition and low switching costs

A high churn rate means:
- Loss of predictable revenue
- Increased acquisition spend
- Reduced customer lifetime value (CLV)

The business needs to know **who is likely to churn and why**, so interventions can happen **before customers leave**.

---

## **Problem Statement**

Analyze telecom customer data to:
- Measure and understand **customer churn**
- Identify **key churn drivers**
- Predict **high-risk customers**
- Support **targeted retention strategies** with maximum ROI

---

## **Hypotheses**

Before analysis, the following hypotheses were framed:

- **H1:** Customers with low tenure are more likely to churn  
- **H2:** Higher monthly charges increase churn risk  
- **H3:** Flexible (month-to-month) contracts lead to higher churn  
- **H4:** Billing preferences and service usage impact churn behavior  

These hypotheses guided both exploratory analysis and modeling.

---

## **Dataset Overview**

- **Total Records:** **7,043 customers**
- **Target Variable:** **Churn (Yes / No)**
- **Churn Distribution:**
  - **73.42% Retained**
  - **26.58% Churned**

**Key Feature Groups:**
- **Demographics:** Gender, SeniorCitizen, Partner, Dependents  
- **Services:** Phone, MultipleLines, Internet, Security, Backup  
- **Account Info:** Tenure, Contract, Payment Method, Monthly Charges  

<img src="https://raw.githubusercontent.com/priyankadatacodes/telco-customer-churn-analysis/main/dashboard/telecom_churn_analysis_dashboard.png" width="100%">

---

## **End-to-End Approach**

<img src="https://raw.githubusercontent.com/priyankadatacodes/telco-customer-churn-analysis/main/churn_workflow.png" width="100%">

### **1. Data Ingestion (MySQL)**
- Imported raw churn dataset from Kaggle  
- Designed relational schema with correct data types  
- Stored data in **MySQL** for integrity and querying  

### **2. Data Extraction & Cleaning (Python)**
- Extracted data using **Pandas + SQLAlchemy**  
- Performed EDA and handled missing values  
- Corrected data types and engineered features  
- Created tenure groups and numeric conversions  

### **3. Analysis & Modeling**
- Performed descriptive churn analysis  
- Identified churn drivers using group statistics  
- Built **Logistic Regression** and **Random Forest** models  
- Generated churn probabilities for each customer  

### **4. Business Dashboarding (Power BI)**
- Built interactive dashboards including:
  - Churn KPIs
  - Customer segmentation
  - High-risk customer identification
  - Feature-level drilldowns  

### **5. Reporting & Documentation**
- Documented business logic, assumptions, and insights in this README  

---

## **Tools & Technologies Used**

- **SQL / MySQL:** Data storage and retrieval  
- **Python:** Pandas, NumPy, Scikit-learn (EDA + modeling)  
- **Power BI:** Interactive dashboards and KPIs  
- **Jupyter Notebook:** Analysis and documentation  

---

## **Key Outcomes**

- **Churn Rate:** **26.58%**
- **Retained Customers:** **73.42%**
- **High-Risk Customers Identified:** **6.33%**
- **Top Churn Drivers:** Low tenure, high monthly charges, digital billing  

---

## **Key Insights**

### **Customer Tenure**
- Median tenure (retained): **38 months**
- Median tenure (churned): **10 months**
- New customers are significantly more likely to churn  

### **Billing & Pricing**
- Median monthly charges:
  - **Retained:** ₹64.5
  - **Churned:** ₹79.7
- Higher bills increase churn likelihood  

### **Revenue Impact**
- Median lifetime charges:
  - **Retained:** ₹1683.6
  - **Churned:** ₹703.5
- Early churn severely reduces lifetime value  

### **Model-Based Risk**
- Average churn probability: **0.27**
- **6.33%** of customers have churn probability > **0.7**
- This segment should be the **top priority** for retention  

---

## **Business Impact**

- Enables proactive churn prevention  
- Supports targeted retention instead of mass campaigns  
- Protects customer lifetime value  
- Reduces revenue leakage from early churn  

---

## **Practical Recommendations**

1. **Improve onboarding for new customers** to reduce early churn  
2. **Review pricing and billing transparency** for high-charge users  
3. **Enhance digital billing clarity** to reduce dissatisfaction  
4. **Focus retention offers on the top 6% high-risk customers**  
5. **Encourage longer-term contracts** with incentives  
6. **Offer basic technical support bundles** for new customers  
7. **Track customer lifetime value (CLV)** alongside churn  

---

## **Final Takeaway**

Customer churn in telecom is driven primarily by **early-stage dissatisfaction, pricing pressure, and contract flexibility**.  
By combining **data analysis and predictive modeling**, the business can move from reactive churn management to **proactive customer retention**, improving both revenue stability and customer satisfaction.

---

## **How to Run**

1. Clone the repository  
2. Install dependencies: `pip install -r requirements.txt`  
3. Run the notebook: `churn_analysis.ipynb`  
4. Open the Power BI dashboard  

---

## **Author**

**Priyanka Lakra**  
**Aspiring Data Analyst | SQL | Python | Power BI**
