# Retail Customer & Sales Analytics: Superstore

Analysis of a US retail dataset (Sample Superstore, 2014–2017) covering
customer segmentation, retention, seasonality, and product profitability —
with business recommendations tied to each finding.

## Headline findings (real, from this dataset)

- **Deep discounts destroy margin.** Profit margin is ~30% at 0% discount
  and falls steadily as discount increases — turning **negative at 21%+
  discounts, and -48% at 30%+**. A large share of Furniture and Technology
  sales fall into these deep-discount tiers.
- **Two sub-categories are unprofitable overall**: Tables (-$17.7K profit on
  $207K revenue) and Bookcases (-$3.5K profit on $115K revenue), despite
  both ranking in the top half of sub-categories by revenue — a case of
  revenue leadership masking margin problems.
- **8 of 17 sub-categories drive ~80% of total revenue** (Phones, Chairs,
  Storage, Tables, Binders, Machines, Accessories, Copiers) — classic
  Pareto concentration, useful for prioritizing merchandising/inventory
  focus.
- Full RFM customer segmentation (Champions / Loyal / Potential Loyalists /
  At Risk / Lost), cohort retention curves, and seasonal revenue patterns
  are in the notebook — see it for the exact splits and dollar figures.

## What's in here

```
├── data/
│   └── superstore_raw.csv        # source data (9,994 line items, 2014-2017)
├── notebook/
│   └── ecommerce_analysis.ipynb  # full analysis, pre-run with all charts
├── charts/                       # exported PNGs of every chart
└── README.md
```

## Dataset

[Sample Superstore](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
— a widely-used real-world US retail dataset: 9,994 order line items,
5,009 orders, 793 customers, January 2014 – December 2017. Each row is a
product line item with Order/Ship dates, Customer, Region/Segment,
Category/Sub-Category, Sales, Quantity, Discount, and Profit.

## How to run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook notebook/ecommerce_analysis.ipynb
```
Or open `notebook/ecommerce_analysis.ipynb` directly on GitHub — it renders
with all charts and tables already visible, no setup needed.

## Analysis covered

1. **Data loading, reshaping & quality checks** — the raw line-item file is
   reshaped into tidy `customers` / `orders` / `items` tables
2. **RFM analysis** — Recency/Frequency/Monetary scoring → 5 customer
   segments, cross-validated with K-Means clustering
3. **Cohort retention analysis** — monthly acquisition cohorts tracked over
   12+ months, visualized as a retention heatmap
4. **Seasonal trends** — monthly revenue trend, year-over-year comparison,
   day-of-week patterns
5. **Product performance** — Pareto (80/20) analysis by sub-category, and
   a discount-level vs. profit-margin analysis
6. **Business recommendations** — five concrete recommendations grounded
   in the analysis: VIP treatment for top-segment customers, a win-back
   campaign for at-risk customers, fixing the month-1 retention drop,
   category investment priorities, and a discount policy cap

## Skills demonstrated

pandas data wrangling & reshaping · RFM segmentation · unsupervised
clustering (K-Means) · cohort/retention analysis · time-series &
seasonality analysis · Pareto analysis · data visualization
(matplotlib/seaborn) · translating analysis into business recommendations
