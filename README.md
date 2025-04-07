# Walmart Black Friday Spending Analysis: Confidence Intervals & CLT

![dataset-cover](https://github.com/user-attachments/assets/536a3e26-5f52-4b2d-a141-f7cbe1f2ca34)

## Project Overview

This project analyzes transactional data from Walmart customers during Black Friday to understand customer purchase behavior, specifically focusing on the purchase amount. The analysis utilizes the Central Limit Theorem (CLT) and Confidence Intervals to compare spending habits between different customer segments (Gender, Marital Status, Age), aiming to provide actionable insights for Walmart's management team.

## Business Problem

Walmart's management seeks to understand if customer spending habits differ significantly across various demographics, particularly during events like Black Friday. Key questions include:
* Do female customers spend more per transaction than male customers on average?
* Can we estimate the average spending of the entire customer population (e.g., 50 million males, 50 million females) based on the sample data?
* Do the average spending ranges (confidence intervals) for different groups (Male vs. Female, Married vs. Unmarried, different Age groups) overlap?
* How can Walmart leverage these findings to make better business decisions regarding marketing, promotions, and inventory?

## Dataset

The dataset (`Walmart_data.csv`) contains transactional information for customers during Black Friday, including:

* User_ID, Product_ID
* Gender, Age (binned), Occupation (masked), City_Category, StayInCurrentCityYears, Marital_Status
* ProductCategory (masked)
* Purchase: Purchase Amount (the target variable for analysis)

* **Source:** [Provide Link to Original Dataset Here if applicable]
* *(Note: The dataset file might/might not be included in the `data/` directory of this repository due to size/privacy constraints. Please refer to the source link if needed.)*

## Repository Structure

```text
Walmart-BlackFriday-Analysis/
├── data/
│   └── Walmart_data.csv  
├── notebooks/
│   └── walmart_clt_analysis.ipynb   
├── reports/                   
│   └── walmart_analysis_report.pdf
├── .gitignore
├── LICENSE 
└── README.md              
```

## Key Findings & Insights 

* **Spending Similarities:** Confidence intervals for average Black Friday spending significantly overlap between male/female customers and between married/unmarried customers, suggesting no statistically meaningful difference in average spending for these population groups.
* **Age Drives Spending:** Clear differences exist across age groups; customers aged 26-50 and 51-55 demonstrate higher average purchase amounts compared to younger (0-17) or older segments.
* **CLT Validation:** The Central Limit Theorem holds, allowing reliable estimation of population average spending using sample data and confidence intervals, despite non-normal individual purchase distributions.

## Recommendations 

*   **Target High-Spending Age Groups:** Focus primary Black Friday marketing efforts and high-value product promotions on the 26-55 age demographic known for higher average spending.
*  **Use Unified Gender/Marital Status Marketing:** Avoid segmenting Black Friday promotions heavily by gender or marital status based *solely* on average spending; use inclusive campaigns instead.
*  **Develop Youth Engagement Strategy:** Create specific offers (e.g., student discounts, starter bundles) to increase engagement and spending potential among the 0-17 age group.
*  **Inform Planning with CIs:** Utilize the calculated confidence interval ranges for average spending across key segments to improve Black Friday sales forecasting and inventory management.


## Tools Used

* **Programming Language:** Python
* **Libraries:** Pandas (Data Manipulation), Matplotlib & Seaborn (Visualization), NumPy, SciPy.stats (for statistical functions, confidence intervals)
* **Environment:** Jupyter Notebook

## License
[Apache License 2.0](LICENSE) 
```
