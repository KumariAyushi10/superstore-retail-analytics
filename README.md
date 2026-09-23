# superstore-retail-analytics

An end-to-end data science and business intelligence project analyzing a US retail dataset (Sample Superstore, 2014–2017). This repository features customer segmentation, cohort retention mapping, seasonal sales analysis, and product profitability modeling with data-driven business recommendations.

## Overview

This project uses Python to uncover hidden performance patterns, analyze customer lifecycles, and evaluate pricing strategy impacts to guide merchandising and operational improvements.

## Business Questions Answered

* **Discount Impacts:** How do promotional markdown strategies across different category tiers impact actual net profit margins?
* **Product Profitability:** Which major revenue-driving product sub-categories are masking hidden losses and destroying company margins?
* **Customer Segmentation:** How can we categorize our user base into actionable groups (Champions, At-Risk, Loyal) based on purchasing behavior?
* **Retention Trends:** What do monthly acquisition cohorts look like when tracked over a 12-month lifecycle?
* **Seasonality Patterns:** How do sales volumes shift across fiscal months, years, and specific days of the week?

## Core Findings

* **Discount Thresholds:** Profit margins remain strong at ~30% with no discount, but collapse into negative returns at markdowns exceeding 21%.
* **Margin Drainers:** High-volume sub-categories like Tables and Bookcases generate significant revenue top-line numbers but remain net unprofitable.
* **Pareto Concentration:** Roughly 80% of total business revenue is driven by just 8 of the 17 product sub-categories.

## Tools & Skills Demonstrated

* **Data Wrangling:** `pandas` and `numpy` for deep cleaning, data reshaping, and metric aggregates.
* **Customer Modeling:** RFM (Recency, Frequency, Monetary) scoring cross-validated using Unsupervised Machine Learning (`scikit-learn` K-Means clustering).
* **Advanced Analytics:** Time-series seasonality tracking, monthly cohort retention matrices, and Pareto (80/20 rule) metrics.
* **Data Visualization:** `matplotlib` and `seaborn` plotting scripts.

## Project Structure

```text
├── charts/            
├── data/              
├── notebook/
│   └── ecommerce_analysis.ipynb  
└── README.md          
```

## How to Run It

To run this notebook environment locally on your machine, you will need [Python 3](https://python.org) installed:

1. Click the green **Code** button at the top of this GitHub page and select **Download ZIP**.
2. Extract the downloaded ZIP file onto your computer.
3. Open your terminal or command prompt, navigate inside the extracted folder, and install the required data stack:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
4. Fire up the notebook environment server:
   ```bash
   jupyter notebook
   ```
5. Navigate into the `notebook/` folder through the browser interface and open `ecommerce_analysis.ipynb`. 

*(Alternatively, you can click on the file directly here inside GitHub to view the pre-rendered analysis text, data tables, and charts instantly without setting up any code libraries locally).*


