
# Automated Data Analysis Report

## Dataset Overview

- Rows: 64374
- Columns: 12
- Column names: customerid, age, gender, tenure, usage_frequency, support_calls, payment_delay, subscription_type, contract_length, total_spend, last_interaction, churn

## Data Quality Check

### Missing Values

{
  "customerid": 0,
  "age": 0,
  "gender": 0,
  "tenure": 0,
  "usage_frequency": 0,
  "support_calls": 0,
  "payment_delay": 0,
  "subscription_type": 0,
  "contract_length": 0,
  "total_spend": 0,
  "last_interaction": 0,
  "churn": 0
}

## Numeric Summary

{
  "customerid": {
    "count": 64374,
    "mean": 32187.5,
    "median": 32187.5,
    "min": 1,
    "max": 64374
  },
  "age": {
    "count": 64374,
    "mean": 41.97,
    "median": 42,
    "min": 18,
    "max": 65
  },
  "tenure": {
    "count": 64374,
    "mean": 31.99,
    "median": 33,
    "min": 1,
    "max": 60
  },
  "usage_frequency": {
    "count": 64374,
    "mean": 15.08,
    "median": 15,
    "min": 1,
    "max": 30
  },
  "support_calls": {
    "count": 64374,
    "mean": 5.4,
    "median": 6,
    "min": 0,
    "max": 10
  },
  "payment_delay": {
    "count": 64374,
    "mean": 17.13,
    "median": 19,
    "min": 0,
    "max": 30
  },
  "total_spend": {
    "count": 64374,
    "mean": 541.02,
    "median": 534,
    "min": 100,
    "max": 1000
  },
  "last_interaction": {
    "count": 64374,
    "mean": 15.5,
    "median": 15,
    "min": 1,
    "max": 30
  },
  "churn": {
    "count": 64374,
    "mean": 0.47,
    "median": 0,
    "min": 0,
    "max": 1
  }
}

## Categorical Summary

{
  "gender": [
    {
      "category": "Female",
      "count": 34353,
      "percentage": 53.36
    },
    {
      "category": "Male",
      "count": 30021,
      "percentage": 46.64
    }
  ],
  "subscription_type": [
    {
      "category": "Standard",
      "count": 21502,
      "percentage": 33.4
    },
    {
      "category": "Basic",
      "count": 21451,
      "percentage": 33.32
    },
    {
      "category": "Premium",
      "count": 21421,
      "percentage": 33.28
    }
  ],
  "contract_length": [
    {
      "category": "Monthly",
      "count": 22130,
      "percentage": 34.38
    },
    {
      "category": "Annual",
      "count": 21410,
      "percentage": 33.26
    },
    {
      "category": "Quarterly",
      "count": 20834,
      "percentage": 32.36
    }
  ]
}

## AI Executive Summary

## Analytical Report on Customer Dataset

### 1. Executive Summary

This dataset appears to measure customer behavior and characteristics, likely related to a subscription-based service. It includes demographic information (age, gender), customer engagement metrics (tenure, usage frequency, last interaction), service interaction data (support calls, payment delay), financial information (total spend), subscription details (subscription type, contract length), and a crucial indicator of customer retention (churn). The dataset comprises 64,374 records and covers 12 distinct attributes.

### 2. Data Quality Assessment

The dataset exhibits excellent data quality with no missing values across all 12 columns. This complete dataset is a significant advantage for analysis. The presence of 64,374 rows suggests a sufficiently large sample size to draw robust conclusions and identify meaningful patterns. The range of values for numeric metrics (e.g., age from 18 to 65, tenure from 1 to 60 months) indicates that the data captures a diverse customer base. The categorical variables (gender, subscription type, contract length) are well-distributed, with each category having a substantial number of observations.

### 3. Metric-Level Analysis

**Numeric Columns:**

*   **customerid:** The mean and median of `customerid` are identical (32187.5), which is expected for sequentially assigned IDs. The min (1) and max (64374) confirm the range of unique customer identifiers. This column is primarily for identification and does not offer analytical insights into customer behavior.
*   **age:** The average age of customers is approximately 42 years, with a median of 42 years. The age range spans from 18 to 65. This suggests the customer base is predominantly in the adult working population.
*   **tenure:** The mean tenure is around 32 months, with a median of 33 months. The tenure ranges from 1 to 60 months, indicating a mix of new and long-term customers. The proximity of mean and median suggests a relatively symmetrical distribution of tenure.
*   **usage_frequency:** On average, customers use the service 15 times per period, with a median of 15. The frequency ranges from 1 to 30. This suggests a moderate level of engagement across the customer base.
*   **support_calls:** The average number of support calls is 5.4, with a median of 6. The range is from 0 to 10 calls. This indicates that while many customers have few or no issues, a portion of the customer base requires significant support.
*   **payment_delay:** The average payment delay is approximately 17 days, with a median of 19 days. The range is from 0 to 30 days. This suggests a notable proportion of customers experience delays in their payments, with some consistently delaying payments up to a month.
*   **total_spend:** The average total spend is $541.02, with a median of $534. The spend ranges from $100 to $1000. The mean and median are close, indicating a somewhat symmetric distribution of total spend.
*   **last_interaction:** The mean and median for last interaction are both 15.5 and 15 respectively. The range is from 1 to 30. This metric likely represents the number of days since the last customer interaction, suggesting a mix of recent and older interactions within the observed period.
*   **churn:** The mean `churn` is 0.47, with a median of 0. The range is 0 to 1, indicating that `churn` is a binary variable (0 for not churned, 1 for churned). The mean of 0.47 suggests that approximately 47% of customers in this dataset have churned. The median of 0 indicates that more than half of the customers have not churned.

### 4. Relationship Hypotheses

*   **Tenure and Total Spend:** Longer tenure might be associated with higher total spend.
*   **Usage Frequency and Total Spend:** Higher usage frequency could correlate with higher total spend.
*   **Support Calls and Churn:** Customers with a higher number of support calls may be more likely to churn.
*   **Payment Delay and Churn:** Customers with significant payment delays might have a higher propensity to churn.
*   **Age and Usage Frequency:** Different age groups might exhibit varying levels of usage frequency.
*   **Contract Length and Churn:** Customers on shorter contract lengths (e.g., Monthly) might have a higher churn rate compared to those on longer contracts (e.g., Annual).
*   **Subscription Type and Total Spend:** Different subscription types (Basic, Standard, Premium) are likely to influence total spend.

### 5. Possible Business or Operational Insights

*   The average age of 42 with a range up to 65 suggests a mature customer base, which might have different service needs and preferences compared to a younger demographic.
*   The moderate average usage frequency (15) indicates that while customers are engaged, there might be opportunities to increase utilization of the service.
*   The average of 5.4 support calls suggests that customer support is a significant touchpoint. High call volumes could indicate underlying issues with the product or service.
*   The average payment delay of 17 days is a considerable concern. This could imply cash flow challenges for the business or indicate customer dissatisfaction or difficulties in managing their accounts.
*   The `churn` rate of approximately 47% is very high and warrants immediate attention. This suggests that a substantial portion of the customer base is not retained.

### 6. Risk Signals

*   **High Churn Rate:** The `churn` mean of 0.47 is a significant warning sign, indicating that almost half of the customers are leaving.
*   **High Support Calls:** An average of 5.4 `support_calls` suggests that a considerable number of customers are experiencing issues significant enough to warrant reaching out to support. This can be a precursor to churn.
*   **Payment Delays:** The `payment_delay` metric, with a mean of 17.13 days, is a clear operational risk. Consistent delays can impact revenue, lead to increased administrative costs for collections, and may be symptomatic of customer dissatisfaction or financial strain, which can contribute to churn.

### 7. Recommended Next Analyses

*   **Correlation Analysis:** Calculate correlation coefficients between numeric variables to quantify the relationships hypothesized in Section 4 (e.g., `tenure` vs. `total_spend`, `support_calls` vs. `churn`, `payment_delay` vs. `churn`).
*   **Categorical-Numeric Analysis:** Analyze the average `churn`, `total_spend`, `usage_frequency`, and `support_calls` for each `subscription_type`, `contract_length`, and `gender`. This will reveal how these categories influence key metrics. For example, compare `churn` rates across different `contract_length` categories.
*   **Visualization:**
    *   Create histograms for `age`, `tenure`, `usage_frequency`, `support_calls`, `payment_delay`, and `total_spend` to understand their distributions.
    *   Generate box plots to visualize `support_calls` and `payment_delay` across different `subscription_type` and `contract_length` categories.
    *   Use bar charts to show the `churn` rate per `gender`, `subscription_type`, and `contract_length`.
*   **Regression Analysis:** Build predictive models (e.g., logistic regression) to understand the drivers of `churn`. This will help identify which factors are most strongly associated with customers leaving.
*   **Segmentation:** Group customers based on combinations of their attributes (e.g., by `subscription_type` and `contract_length`, or by `age` and `usage_frequency`) to identify high-risk or high-value segments. Analyze `churn` rates within these segments.
*   **Time Series Analysis (if applicable):** If `last_interaction` can be mapped to specific dates or periods, analyze trends in `usage_frequency`, `support_calls`, `payment_delay`, and `churn` over time to identify seasonal patterns or emerging issues.

### 8. Final Analyst Takeaway

This dataset reveals a customer base where a significant portion is experiencing payment delays and a high rate of churn. Understanding the interplay between customer engagement, service interactions, and subscription details is crucial to address these critical issues and improve customer retention.

## Recommended Next Steps

- Review missing values and possible outliers.
- Add correlation analysis in the next version.
- Add visual charts in the next version.
- Compare groups if the dataset contains useful categories.

Generated automatically with n8n.
