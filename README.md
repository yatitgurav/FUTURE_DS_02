# FUTURE_DS_02 - Customer Churn & Retention Analysis

## Objective

Analyze customer subscription data to understand churn patterns, identify key retention drivers, study customer lifetime trends, and generate actionable business insights to reduce customer loss.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset

The project uses a **Customer Churn & Retention Dataset** containing customer subscription information.

The analysis uses fields such as:

- Customer ID
- Signup Date
- Churn Status
- Churn Date
- Subscription Plan
- Contract Type
- Tenure
- Monthly Charges
- Payment Method
- Technical Support
- Churn Reason

## Project Workflow

### 1. Data Loading

The customer churn dataset is loaded into Python using Pandas.

### 2. Data Inspection

The dataset is inspected using:

- Dataset shape
- First few records
- Data types
- Missing values
- Summary statistics

### 3. Data Cleaning

The following preprocessing steps were performed:

- Removed duplicate customers using `CustomerID`
- Removed extra spaces from column names
- Converted `SignupDate` and `ChurnDate` into datetime format
- Converted numerical columns into numeric format
- Removed records with missing essential values
- Standardized the `Churn` column
- Filled missing monthly charges using the median

### 4. Churn & Retention Analysis

The project calculates:

- Total customers
- Churned customers
- Retained customers
- Churn rate
- Retention rate

### 5. Churn by Subscription Plan

Churn rates are analyzed across different subscription plans to identify customer segments with different observed churn levels.

### 6. Churn by Contract Type

Customer churn is compared across contract types, including month-to-month customers.

### 7. Churn by Customer Tenure

Customers are grouped into tenure ranges:

- 1–12 Months
- 13–24 Months
- 25–36 Months
- 37–48 Months

The observed churn rate is analyzed for each group.

### 8. Churn Reasons

The project analyzes recorded churn reasons such as:

- Price
- Support
- Product Features
- Competitor
- Moved/Not Needed

### 9. Payment Method Analysis

Churn rates are compared across different payment methods.

### 10. Technical Support Analysis

The analysis compares churn between customers with different technical support statuses.

### 11. Monthly Charges Analysis

Monthly charges are compared between churned and retained customers using statistical summaries and a box plot.

### 12. Customer Lifetime Analysis

Average and median customer lifetime are analyzed using customer tenure.

### 13. Signup Cohort Analysis

Customers are grouped according to their signup month to analyze observed retention patterns across different customer cohorts.

## Key Business Insights

1. The analysis measures overall customer churn and retention to understand the current customer base.

2. Churn varies across different subscription plans, helping identify customer segments with higher observed customer loss.

3. Contract type shows differences in observed churn, with month-to-month customers requiring particular attention.

4. Customer tenure provides insights into customer lifetime and helps identify early and long-term retention patterns.

5. Churn rates vary across payment methods and can be investigated further for customer-experience or payment-related issues.

6. Customers with and without technical support show differences in observed churn rates.

7. Recorded churn reasons include Price, Support, Product Features, Competitor, and Moved/Not Needed.

8. Signup cohort analysis helps compare observed retention patterns among customers who joined during different periods.

9. Monthly charges can be compared between churned and retained customers to understand differences in customer spending.

10. Customer lifetime analysis provides an overview of the average and median tenure of churned and retained customers.

## Business Recommendations

1. Focus on customer segments with higher observed churn and develop targeted retention strategies.

2. Improve onboarding and customer engagement, especially during the early subscription period.

3. Monitor month-to-month customers and consider suitable long-term subscription incentives.

4. Improve technical support and proactively address customer service issues.

5. Investigate pricing-related churn and review whether subscription plans provide appropriate value.

6. Analyze product feature feedback to identify improvements that could reduce customer loss.

7. Monitor payment-method-specific churn patterns and investigate potential payment or customer-experience issues.

8. Use customer tenure and cohort information to identify customers who may require additional retention support.

9. Regularly monitor churn reasons and retention metrics to identify changing customer behavior.

10. Validate retention strategies using future customer data and controlled experiments before applying them as fixed business rules.

## Project Outputs

The notebook also exports analysis results into CSV files:

- `churn_summary.csv`
- `churn_by_plan.csv`
- `churn_by_contract.csv`
- `churn_by_tenure.csv`
- `churn_by_payment.csv`
- `churn_by_support.csv`
- `signup_cohort_analysis.csv`

## Conclusion

This project analyzed customer subscription data to understand customer churn, retention, churn reasons, and customer lifetime trends.

The analysis examined churn across subscription plans, contract types, customer tenure, payment methods, technical support, monthly charges, and signup cohorts.

The findings provide a structured understanding of customer behavior and highlight customer segments and factors associated with different observed churn rates.

These insights can support data-driven retention strategies by helping businesses improve onboarding, strengthen customer support, investigate pricing and product issues, and monitor high-churn customer segments.

The findings represent relationships observed in the dataset and should be validated with additional business data or controlled experiments before being treated as causal business rules.

## Track Information

**Track:** Data Science & Analytics  
**Task:** Task 2  
**Repository:** FUTURE_DS_02
