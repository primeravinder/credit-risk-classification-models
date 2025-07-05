# Credit Risk Modeling Project

## Project Overview  
**The Client Bank (Europe)** received **1.4 million credit/loan applications**. Out of these, **0.45 million customers** were granted credit, leading to a total loan amount of **$6.5 billion**.  
However, **40,000 customers defaulted**, resulting in a total default amount of **$510 million** (~8% of the total loan amount). Although this is within regulatory norms (CRAR, Basel II Norms), It raises concerns of increased scrutiny from banking regulators.

## Challenges Faced by the Bank  
- **Increased Capital Risk Adequacy Ratio (CRAR):** More capital must be set aside, reducing available funds for new loans.  
- **Decreased Profitability:** Less lending means a direct impact on business revenue.  
- **Regulatory Pressure:** Stricter compliance rules due to increased defaults.  

## What is Credit Risk?  
Credit risk arises when a borrower fails to pay back their loan fully or partially.  

- **Data Period:** 2009 - 2019 (10 Years)  

## Project Objectives  
- Predict the **Expected Loss (EL)** and minimize risk.  
- Improve profitability while maintaining regulatory compliance.  

**Formula:**  
EL = PD × LGD × EAD

Where:  
- **PD:** Probability of Default  
- **LGD:** Loss Given Default  
- **EAD:** Exposure at Default  

## Challenges in Model Development  
- **Highly Imbalanced Dataset**  
- **Data Quality Issues:** Missing values, unstructured data, alternative credit scores  
- **Regulatory Restrictions:** Some data requires special approval  
- **Model Bias:** Biases in the training data could affect predictions  
- **Model Interpretability vs Accuracy Trade-off**

## Key Performance Indicators (KPIs)  
- **Primary Metrics:** Gini Coefficient, KS Statistic  
- **Secondary Metrics:** Precision  

## Project Workflow  
1. **Data Extraction:** SQL  
2. **Data Preprocessing:** Python, Pandas  
3. **Exploratory Data Analysis (EDA):** Pandas, Matplotlib, Seaborn  
4. **Feature Engineering:** Weight of Evidence (WoE), Information Value (IV)  
5. **Model Development:**  
   - PD Model: Logistic Regression to predict probability of default  
   - EAD Model: Linear Regression to estimate exposure at default  
6. **Model Evaluation:** ROC, AUC, Gini Coefficient, Kolmogorov-Smirnov Test  
7. **Model Deployment:** Integrated with the bank's transaction system  
8. **Model Monitoring:** Population Stability Index (PSI) — if PSI > 0.25, further investigation is needed

## Tools & Technologies Used  
- **Data Extraction:** SQL  
- **Data Handling & Processing:** Python, Pandas  
- **Visualization:** Matplotlib, Seaborn, Power BI  
- **Machine Learning:** Scikit-Learn, Logistic Regression, Linear Regression

## Stakeholders  
- The Bank & Domain Experts  
- Project Development Team  
- Product Manager  
- Software Engineers  
- Data Scientists

## Project Results  
- **Model Precision:** 70% in identifying Probability of Default  
- **Profitability Increase:** 10% improvement compared to the previous year  
