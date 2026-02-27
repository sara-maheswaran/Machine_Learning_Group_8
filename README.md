# Machine_Learning_Group_8

## Project Title
Customer Segmentation for Targeted Marketing Optimization


## Project Overview
This project utilizes advanced machine learning techniques to transition marketing strategies from generalized outreach to highly targeted, data-driven campaigns. The analysis is split into two core objectives: identifying hidden customer segments through unsupervised clustering, and building predictive classification models to determine a customer’s likelihood to accept future promotions. Ultimately, this approach empowers the business to allocate marketing spend efficiently, maximize campaign ROI, and engage the right customers with the right offers.

## Business Problem
The company currently applies broad, non-personalized marketing campaigns across its entire customer base. This leads to:

- Inefficient marketing spend
    * Utilizing a generalized strategy increases marketing spend by wasting budget on demographic segments with a near-zero probability of conversion
- Low campaign conversion rates
    * One-size-fits-all approaches for campaigns results in ignored promotions and stagnant sales throughput, despite high-volume outreach
- Poor differentiation between high-value and low-value customers
    * Without customer segmentation, customers who are highly profitable are treated the same as one-off buyers, thus leaving revenue streams open to competitor offers 
- Missed upselling and retention opportunities
    * High-probability cross-sell opportunities are missed and instead the company waits for customers to churn before trying to save them

There is a critical need for data-driven segmentation and predictive modeling to understand customer behavior, anticipate their actions, and tailor marketing strategies accordingly.

## Stakeholders
The primary audience is:
- Marketing Managers
    * Customer segmentation will allow marketing managers to know who their most profitable customers are and how to reach them efficiently with ads tailored to their purchasing habits
- CRM / Customer Experience Teams
    * Loyalty programs and automated emails with tailored campaigns can be developed to decrease recency and build re-engagement where needed
- Business Strategy Executives
    * Overall company business strategies can be driven based on customer purchasing behaviour
- Sales Leadership
    * Insights into where customers make purchases can guide where investments can be made to increase sales - ex. store expansions vs e-commerce infrastructure 

Secondary audience:
- Data team / Analytics team (for implementation)
    * Results from clustering and the models created can be used to update other tools used by the company as required (ex. Salesforce), modify to process larger datasets, or retrain the model when new data is available

## Business Objective
The primary objective of this project is to:
- Identify distinct customer clusters using purchasing and demographic data.
- Improve marketing targeting strategies.
- Increase campaign effectiveness and ROI.
- Support long-term customer retention and revenue growth.

Success is measured through cluster interpretability, internal validation metrics, and business usefulness of the segments.

## Dataset Description
### Source: [Kaggle – Customer Personality Analysis Dataset](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis?resource=download)
The dataset contains customer demographic information, purchasing behavior, and campaign response history.
### Shape
- Rows: 2,240 customers
- Columns: 29 variables

Each row represents a unique customer, and each column represents demographic information, purchasing behavior, or campaign interaction history.

### Key Variables Categories:
### Demographics
- Income
- Year_Birth
- Education
- Marital_Status
- Kidhome, Teenhome (Number of Children)
### Spending Behavior
Amount spent on wines, fruits, meat, fish, sweets, and gold products:
- MntWines
- MntFruits
- MntMeatProducts
- MntFishProducts
- MntSweetProducts
- MntGoldProds
### Purchase Behavior/Channels
- NumWebPurchases (Web purchases)
- NumCatalogPurchases (Catalog purchases)
- NumStorePurchases (Store purchases)
- NumWebVisitsMonth (Website visits per month)
### Engagement
- Recency (days since last purchase)
- AcceptedCmp1–AcceptedCmp5 (Campaign acceptance indicators)
- Response (target variable: campaign acceptance)

## Risks and Unknowns
### Risks
- Poor Cluster Interpretability: Clusters may not be clearly distinct or actionable.
Mitigation: Use validation metrics, limit cluster count, perform clear profiling, and validate with business stakeholders.

- Data Quality Issues: Missing income values, Outliers (extreme spending), Inaccurate customer demographics
Mitigation: Clean data systematically (imputation, outlier treatment), conduct EDA, and document preprocessing steps.

- Over-Segmentation: Too many clusters may confuse marketing teams and/or complicate execution.
Mitigation: Select optimal cluster number using statistical methods and align with business execution capacity.

- Static Segmentation: Customer behavior changes over time.
Mitigation: Retrain models periodically and incorporate recency-based features to capture behavioral changes.

- External Factors: Economic downturn, seasonality, product changes may impact behavior.
Mitigation: Monitor model performance over time and reassess assumptions during economic or seasonal shifts.

### Unknowns
- True customer lifetime value (CLV)
- Customer satisfaction levels
- Competitor influence
- Macro-economic conditions
- Marketing budget constraints






