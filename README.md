# Telecom Customer Churn Analysis

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python\&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0%2B-4479A1?logo=mysql\&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Analytics-orange?logo=mysql)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi\&logoColor=black)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Logistic%20Regression%20%7C%20Random%20Forest-success)

## Executive Summary

End-to-end **telecom customer churn analytics project** focused on identifying high-risk customers, understanding churn drivers, and supporting targeted retention strategies.

The project combines **MySQL, Python, SQL, Machine Learning, and Power BI** across the full analytics workflow—from data ingestion and cleaning to predictive modeling and business reporting.

### Business Question

> **Which customers are most likely to churn, what factors drive churn, and where should retention efforts be focused?**

The analysis covers **7,043 customers**, with an overall churn rate of **26.58%**.

---

## 1. Business Problem

Telecom businesses depend on recurring subscription revenue and long-term customer relationships. High customer churn can result in:

* Revenue loss
* Increased customer acquisition costs
* Lower customer lifetime value
* Reduced revenue predictability

The project analyzes customer behavior to measure churn, identify key drivers, predict high-risk customers, and support targeted retention strategies.

---

## 2. Analytical Hypotheses

The analysis was structured around four hypotheses:

* **H1:** Customers with lower tenure are more likely to churn
* **H2:** Higher monthly charges increase churn risk
* **H3:** Month-to-month contracts are associated with higher churn
* **H4:** Billing preferences and service usage influence churn behavior

These hypotheses guided the exploratory analysis and predictive modeling.

---

## 3. Dataset

| Attribute       | Details              |
| --------------- | -------------------- |
| Dataset         | Telco Customer Churn |
| Total Customers | **7,043**            |
| Target Variable | `Churn`              |
| Retained        | **73.42%**           |
| Churned         | **26.58%**           |

### Feature Groups

**Demographics**

* Gender
* SeniorCitizen
* Partner
* Dependents

**Services**

* Phone
* MultipleLines
* Internet
* Security
* Backup

**Account Information**

* Tenure
* Contract
* Payment Method
* Monthly Charges

---

## 4. Analytics Workflow

```text
Raw Kaggle Dataset
        ↓
MySQL Data Ingestion
        ↓
Schema & Data Validation
        ↓
Python Data Cleaning
        ↓
Exploratory Data Analysis
        ↓
Feature Engineering
        ↓
Churn Analysis & Modeling
        ↓
Churn Probability Scoring
        ↓
Power BI Dashboard
        ↓
Retention Insights
```

The project follows an end-to-end workflow combining data engineering, descriptive analytics, predictive modeling, and business intelligence.

---

## 5. Data Preparation

### MySQL

* Imported the raw churn dataset
* Designed the relational schema
* Applied appropriate data types
* Stored the dataset in MySQL for querying and analysis

### Python

Using **Pandas + SQLAlchemy**:

* Extracted data from MySQL
* Performed exploratory analysis
* Handled missing values
* Corrected data types
* Created numeric features
* Created tenure groups

---

## 6. Churn Analysis & Machine Learning

Two classification approaches were used:

### Logistic Regression

Used to analyze relationships between customer characteristics and churn probability.

### Random Forest

Used as an additional classification approach for churn prediction.

### Customer Risk Scoring

The models generate churn probabilities for individual customers, allowing the analysis to identify customers with elevated churn risk.

The project uses predictive modeling for **analytical insight and customer-risk identification**, rather than production deployment.

---

## 7. Power BI Dashboard

The Power BI reporting layer provides interactive analysis of:

* Churn KPIs
* Customer segmentation
* High-risk customers
* Churn-driver analysis
* Feature-level drilldowns

The dashboard translates analytical results into a business-facing view for customer retention analysis.

### Dashboard Preview

![Telecom Customer Churn Dashboard](https://raw.githubusercontent.com/priyankadatacodes/telco-customer-churn-analysis/main/dashboard/telecom_churn_analysis_dashboard.png)

---

## 8. Key KPIs

| KPI                       |     Result |
| ------------------------- | ---------: |
| Total Customers           |  **7,043** |
| Retained Customers        | **73.42%** |
| Churned Customers         | **26.58%** |
| Overall Churn Rate        | **26.58%** |
| High-Risk Customers       |  **6.33%** |
| Average Churn Probability |   **0.27** |

---

## 9. Key Findings

### Customer Tenure

| Metric        |      Retained |       Churned |
| ------------- | ------------: | ------------: |
| Median Tenure | **38 months** | **10 months** |

Customers with shorter tenure show substantially higher observed churn.

### Monthly Charges

| Metric                 |  Retained |   Churned |
| ---------------------- | --------: | --------: |
| Median Monthly Charges | **₹64.5** | **₹79.7** |

Higher monthly charges are associated with higher observed churn.

### Customer Lifetime Value

| Metric                  |     Retained |    Churned |
| ----------------------- | -----------: | ---------: |
| Median Lifetime Charges | **₹1,683.6** | **₹703.5** |

Early churn substantially reduces accumulated customer lifetime charges.

### Model-Based Risk

* Average churn probability: **0.27**
* **6.33%** of customers have churn probability above **0.70**
* This segment represents the defined high-risk customer group for retention analysis

---

## 10. Key Churn Drivers

The analysis identifies the following major churn patterns:

* **Low customer tenure**
* **Higher monthly charges**
* **Month-to-month contract structure**
* **Digital billing**
* Early-stage customer dissatisfaction

The project combines descriptive analysis and predictive modeling to identify these patterns.

---

## 11. Business Impact

The analysis supports:

* Proactive churn prevention
* Targeted retention instead of broad customer campaigns
* Customer lifetime value protection
* Identification of high-risk customer segments
* Reduced revenue leakage from early customer churn

---

## 12. Retention Recommendations

1. **Improve onboarding** for new customers to address early-stage churn.
2. **Review pricing and billing transparency** for customers with higher monthly charges.
3. **Improve digital billing clarity** where billing behavior is associated with churn.
4. Focus retention efforts on the defined **high-risk customer segment**.
5. Encourage **longer-term contracts** through appropriate incentives.
6. Provide **technical support bundles** for newer customers.
7. Track **Customer Lifetime Value alongside churn** to evaluate retention impact.

---

## 13. Project Structure

```text
telco-customer-churn-analysis/
│
├── dashboard/
│
├── data/
│
├── notebook/
│   └── churn_analysis.ipynb
│
├── sql/
│
├── churn_workflow.png
├── telecom_churn_analysis.png
├── requirements.txt
└── README.md
```

The repository contains dedicated areas for dashboard assets, data, notebooks, and SQL analysis.

---

## 14. How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/priyankadatacodes/telco-customer-churn-analysis.git
cd telco-customer-churn-analysis
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Analysis

Open and execute:

```text
notebook/churn_analysis.ipynb
```

### 4. Open the Power BI Dashboard

Open the project dashboard to explore churn KPIs, customer segmentation, risk identification, and churn-driver analysis.

---

## 15. Skills Demonstrated

### Data Analytics

* Customer Churn Analysis
* Exploratory Data Analysis
* Customer Segmentation
* KPI Analysis
* Business Insight Generation

### Python

* Pandas
* NumPy
* SQLAlchemy
* Scikit-learn
* Feature Engineering
* Predictive Modeling

### SQL

* MySQL
* Data Storage
* Data Extraction
* Analytical Queries

### Machine Learning

* Logistic Regression
* Random Forest
* Binary Classification
* Churn Probability Scoring

### Business Intelligence

* Power BI
* KPI Dashboards
* Customer Risk Analysis
* Feature-Level Drilldowns

---

## 16. Limitations

* The project is based on the available telecom churn dataset.
* Predictive models are used for analytical insight rather than production deployment.
* Observed relationships should be interpreted as associations within the dataset rather than proof of causation.
* Retention recommendations are based on patterns identified in the available customer data.

---

## 17. Future Improvements

Potential extensions include:

* Model performance comparison and tuning
* Explainable ML for churn predictions
* Customer Lifetime Value modeling
* Automated churn-risk scoring
* Customer-level retention prioritization
* Automated reporting pipelines
* Production deployment of the churn model

---

## 18. Author

**Priyanka Lakra**
Data Analyst | SQL · Python · Power BI

**Portfolio:** [bloomindata.in](https://www.bloomindata.in/)

**GitHub:** [priyankadatacodes](https://github.com/priyankadatacodes)

---

## License

This project is available under the repository's existing license.
