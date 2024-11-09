# Credit-Card-Usage-and-Customer-Profile-Analysis

This project aims to analyze credit card usage patterns and customer demographics to identify trends, predict behaviors, and assist in targeted marketing strategies. By evaluating transactional data alongside demographic profiles, the analysis offers insights into credit card utilization, customer satisfaction, and account management for improved decision-making.

---

### Objectives

1. **Understand Customer Demographics**: Identify key characteristics such as age, education, income, and marital status to profile different customer segments.
2. **Analyze Spending Patterns**: Examine transaction volumes, transaction types (e.g., grocery, fuel), and spending frequency to understand credit card usage behaviors.
3. **Assess Credit Card Features and Usage**: Investigate annual fees, credit limits, and utilization ratios to determine their impact on customer satisfaction and loyalty.
4. **Explore Risk and Profitability**: Identify factors related to delinquency, interest earned, and customer acquisition costs to optimize credit risk assessment and profitability.
5. **Customer Satisfaction and Retention**: Analyze satisfaction scores in relation to transaction patterns, card features, and demographic factors to recommend strategies for retention.

---

### Data Description

1. **Credit Card Dataset**:
   - **Client_Num**: Unique identifier for each customer.
   - **Card_Category**: Type of credit card held (e.g., Blue, Silver).
   - **Annual_Fees**: Annual fee for holding the card.
   - **Activation_30_Days**: Whether the card was activated within the first 30 days.
   - **Customer_Acq_Cost**: Customer acquisition cost.
   - **Week_Start_Date / Week_Num / Qtr / current_year**: Temporal variables for tracking the period of transactions.
   - **Credit_Limit**: Credit limit of the customer.
   - **Total_Revolving_Bal**: Revolving balance for the customer.
   - **Total_Trans_Amt / Total_Trans_Vol**: Total transaction amount and volume.
   - **Avg_Utilization_Ratio**: Average utilization ratio.
   - **Use Chip / Exp Type**: Type of card usage and expenditure type.
   - **Interest_Earned**: Interest earned from the customer.
   - **Delinquent_Acc**: Delinquency status of the account.

2. **Customer Dataset**:
   - **Client_Num**: Matches the credit card dataset.
   - **Customer_Age**: Age of the customer.
   - **Gender / Dependent_Count / Education_Level / Marital_Status**: Demographic variables.
   - **state_cd / Zipcode**: Geographic indicators.
   - **Car_Owner / House_Owner / Personal_loan**: Asset and loan indicators.
   - **contact**: Contact method.
   - **Customer_Job**: Occupation of the customer.
   - **Income**: Annual income.
   - **Cust_Satisfaction_Score**: Customer satisfaction score (1-5 scale).

---

### Workflow

1. **Data Preprocessing**:
   - Merge both datasets on `Client_Num`.
   - Handle missing values, particularly for demographics and income fields.
   - Convert categorical variables like `Card_Category`, `Education_Level`, and `Marital_Status` into numerical or dummy variables for analysis.

2. **Exploratory Data Analysis (EDA)**:
   - Analyze customer demographics and spending patterns.
   - Investigate the distribution of transaction types, credit limits, and utilization ratios.
   - Segment customers based on satisfaction scores, annual fees, and acquisition costs.

3. **Feature Engineering**:
   - Create additional metrics like spending-to-income ratios, revolving balance proportions, and loyalty indicators (based on satisfaction score).
   - Categorize customers based on risk by combining delinquency, credit limit utilization, and income.

4. **Predictive Analysis**:
   - Build models to predict customer delinquency or high spending behavior based on demographics, credit card features, and transactional patterns.
   - Segment high-value customers by combining high satisfaction scores, high credit limits, and consistent spending behaviors.

5. **Interpretation and Insights**:
   - Derive insights from EDA and predictive modeling to identify key drivers for customer satisfaction, loyalty, and profitability.

---

### Key Findings

1. **Customer Segmentation**:
   - Identified primary customer segments based on demographic characteristics, spending behavior, and card usage patterns.
   - Younger customers with higher credit limits showed higher transaction volumes but often had lower satisfaction scores due to higher fees.

2. **Card Usage Patterns**:
   - Customers in certain occupations (e.g., Businessman and Self-employed) had a higher frequency of travel and fuel-related transactions, indicating higher utilization for specific categories.
   - The `Avg_Utilization_Ratio` significantly impacted interest earned and delinquency likelihood.

3. **Satisfaction and Retention Factors**:
   - Satisfaction scores correlated positively with credit limits and negatively with high annual fees.
   - Customers who owned a car and house showed higher satisfaction scores, likely due to financial stability.

4. **Delinquency Risks**:
   - Delinquent accounts were more prevalent among customers with high utilization ratios and low income, indicating potential risk factors.
   - Occupations with irregular income (e.g., self-employed) had a higher likelihood of delinquency.

---

### Conclusion

This credit card analysis provides actionable insights into customer spending, credit utilization, and demographic factors influencing satisfaction and retention. Key findings point toward the importance of tailoring credit limits and fees to match customer profiles, especially for high-value customer retention. By focusing on predictive models for delinquency, the company can also enhance its risk management strategies. 

Future work could involve a more granular examination of transaction categories and dynamic modeling to capture seasonal changes in customer behavior. Overall, the analysis offers a robust framework for data-driven decision-making in customer relationship management and credit card portfolio optimization.
