# Customer Churn Analysis

## Objective
The primary objective of this project is to analyze customer churn using data visualization and exploratory data analysis (EDA) techniques. The analysis aims to understand customer behavior, identify patterns in churn, and derive insights that can help improve business operations and customer retention strategies. The focus is on understanding the relationship between various customer attributes and the likelihood of churn.

## Data Cleaning
The dataset contains information on customer details, subscription plans, payment methods, and service usage. Below are the steps taken for data cleaning:

1. **Handling Missing Data**: 
   - Missing values in the `TotalCharges` column were replaced with `0` since a blank space in `TotalCharges` signifies no charges recorded.
   
2. **Data Type Conversion**:
   - The `TotalCharges` column, originally in string format, was converted to `float` for accurate numerical analysis.

3. **Duplicate Checking**: 
   - Checked for duplicate records using the `customerID` column to ensure data integrity.

## Exploratory Data Analysis (EDA)
The dataset was analyzed using several EDA techniques, including data visualization and statistical summaries:

1. **Data Overview**: 
   - The `df.info()` and `df.describe()` methods were used to inspect the data, check for null values, and summarize basic statistics.
   
2. **Visualizations**:
   - **Churn Distribution**: The `countplot` was used to visualize the distribution of customers based on churn status (`Churn` column).
   - **Churn Percentage**: A pie chart shows the percentage of customers who churned out of the total customer base.
   - **Senior Citizen vs. Churn**: A `countplot` was used to compare churn rates between senior and non-senior citizens.
   - **Tenure vs. Churn**: A histogram was created to show the relationship between customer tenure (length of time using the service) and churn.
   - **Contract Type vs. Churn**: A `countplot` was used to assess the relationship between contract type and churn. Customers with month-to-month contracts were more likely to churn.
   - **Payment Method vs. Churn**: A `countplot` visualized the impact of payment methods on churn. Customers using electronic checks were more likely to churn.

## Findings
- **Total Sales**: The dataset contains information on customers and their churn behavior. 
- **Customer Retention**: Customers with long-term contracts (1-2 years) are more likely to stay, while those on month-to-month contracts are more likely to churn.
- **Senior Citizens**: Senior citizens exhibit different churn patterns compared to other customers. The `SeniorCitizen` column was converted to a human-readable format, revealing a notable relationship between age and churn behavior.
- **Tenure vs. Churn**: Customers who have been with the company for a longer period (tenure) tend to stay, while those with shorter tenures (1-2 months) have a higher churn rate.
- **Payment Method**: Customers using electronic checks are more likely to churn, indicating that this payment method may be linked to dissatisfaction.

## Insights
- **Customer Retention Strategy**: Offering longer-term contracts or better incentives for month-to-month customers could improve retention rates.
- **Senior Citizens**: Targeting senior citizens with personalized offers or better support may reduce churn in this demographic.
- **Payment Method**: Improving the user experience for customers using electronic checks could help reduce churn in that segment.

## Conclusion
This analysis highlights key patterns that businesses can leverage to reduce churn and enhance customer retention. Understanding the factors that contribute to churn (such as contract type, tenure, and payment methods) allows the company to tailor its marketing strategies, improve customer service, and offer customized plans to high-risk segments, such as month-to-month contract holders and customers using electronic checks.

### Recommendations for Business Growth:
- **Optimize Offerings for Senior Citizens**: Senior citizens could be offered better incentives to improve retention.
- **Improve Contract Options**: Encourage customers to opt for long-term contracts by providing additional benefits.
- **Enhance Payment Method Experience**: Address issues related to electronic check payments, possibly offering alternative payment methods to reduce churn.
  
This analysis, powered by customer data, provides actionable insights to improve business performance and customer satisfaction.
