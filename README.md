# Pharma-drug-sales-analysis
## Pharma Sales Analysis & Power BI Dashboard

Python + Power BI analysis of 2,106 daily pharmaceutical sales records (2014–2019), digging into product concentration, seasonality, and time-of-day patterns, then turned into a two-page interactive dashboard.

## Data

- 2,106 daily observations, 2014–2019
- **Source:** [Kaggle — Pharma Sales Data](https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data)

## What I did

**Exploratory analysis**
- Daily, monthly, and annual sales trends
- Day-of-week and hourly sales patterns
- Product contribution and product performance by year
- Outlier and distribution checks

**Statistical testing**
- Descriptive stats and product-to-product correlation
- One-way ANOVA + Tukey HSD, run separately for products and for years
- Linear regression to test for a long-term sales trend
## Dashboard

**Page 1 — Sales Overview**

![Sales Overview Dashboard](dashboard/dashboard_page1.png)

**Page 2 — Business Insights**

![Business Insights Dashboard](dashboard/dashboard_page2.png)



## Repo structure

```text
├── data/
│   ├── salesdaily.csv
│   └── saleshourly.csv
├── notebooks/
│   └── Final_analysis.ipynb
├── dashboard/
│   ├── pharma_sales_analysis_dashboard.pbix
│   ├── dashboard_page1.png
│   └── dashboard_page2.png
├── README.md
└── LICENSE
```
## How to run

Clone the repository:

```bash
git clone https://github.com/khushiSdhok/Pharma-drug-sales-analysis.git
cd Pharma-drug-sales-analysis
```

Install the required Python packages:

```bash
pip install pandas numpy scipy matplotlib seaborn jupyter
```

Run the notebook:

```bash
jupyter notebook notebooks/Final_analysis.ipynb
```

Open `dashboard/pharma_sales_analysis_dashboard.pbix` in Power BI Desktop to explore the interactive dashboard.

## Tools

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Power BI
- DAX

## Limitations / Next Steps

- No statistically significant linear trend was found across the full time range.
- Future analysis could test for structural breaks or seasonality-adjusted trends.
- Product-level drivers behind the 2019 sales decline could be investigated further.
