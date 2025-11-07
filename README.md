### Customer-churn-prediction
Customer churn refers to the situation  whereby customers stop doing business with a company. Predicting churn helps businesses understand which customers are likely to leave so they can take action to retain them. Customer churn prediction is crucial in the sales industry as it enables businesses to identify customers who are likely to stop doing business with them. 

### Objective

To build a machine learning model that predicts customer churn using RFM (Recency, Frequency, Monetary) analysis.

### Dataset Overview

The dataset includes key business and customer attributes such as:
Row ID, Order ID, Order Date, Ship Date, Ship Mode
Customer ID, Segment, Country, City, State, Postal Code, Region
Product ID, Category, Sub-Category, Product Name, Sales

### Project Workflow

**RFM Analysis**

Calculated Recency, Frequency, and Monetary scores for each customer.

Visualized customer segments based on their purchasing behavior.

**Churn Labeling**

Defined churn based on purchase inactivity and engagement behavior.

Found that 74.65% of customers are active, while 25.35% are churned.

**Feature Engineering**

Features: R (Recency), F (Frequency), M (Monetary)

Target: Churn (1 = churned, 0 = active)

Standardized the features using StandardScaler.

**Model Building**

Trained and evaluated three models:

Logistic Regression

Random Forest

XGBoost

**Evaluation**

Compared model accuracies and performance metrics.

Model	Accuracy
Logistic Regression	91.0%
Random Forest	95.5%
XGBoost	96.0%

### Results & Insights

XGBoost delivered the highest accuracy (96%), demonstrating excellent predictive performance.

Random Forest also performed strongly, offering interpretability and robustness.

RFM analysis proved effective for segmenting and understanding customer churn behavior.

###  Confusion Matrix Analysis
From the confusion matrix, it is observed that:

- The model correctly predicted a high number of **active customers (True Negatives)**.  
- It also accurately captured **most of the churned customers (True Positives)**.  
- The **False Positives** and **False Negatives** were minimal, indicating strong generalization.  

This shows that the churn prediction model is effective at distinguishing between active and churned customers.



