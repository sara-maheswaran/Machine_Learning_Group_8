# Machine_Learning_Group_8

## Project Title
Customer Segmentation for Targeted Marketing Optimization


## Project Overview
This project applies unsupervised machine learning techniques to segment customers based on purchasing behavior, demographics, and campaign engagement. The objective is to identify distinct customer groups that enable targeted marketing strategies and improved business decision-making. Through feature engineering, clustering, and evaluation metrics, we aim to generate actionable insights that improve targeted marketing strategies and optimize business performance.

## Business Problem
The company currently applies broad, non-personalized marketing campaigns across its entire customer base. This leads to:

- Inefficient marketing spend
- Low campaign conversion rates
- Poor differentiation between high-value and low-value customers
- Missed upselling and retention opportunities

There is a need for data-driven segmentation to better understand customer behavior and tailor strategies accordingly.

## Stakeholders
The primary audience is:
- Marketing Managers
- CRM / Customer Experience Teams
- Business Strategy Executives
- Sales Leadership

Secondary audience:

- Data team / Analytics team (for implementation)

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






