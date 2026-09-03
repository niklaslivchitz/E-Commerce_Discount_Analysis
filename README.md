# E-Commerce Discount Analysis

## Project Overview
Analysis of a fictional company's discount strategy using Python (Pandas/Seaborn). 
The dataset was synthetically corrupted to simulate real-world data quality challenges.
Completed as a data analytics bootcamp project, working in a small group; individual analysis and additional plotting were done independently (see discount_analysis/ and discount_analysis_seaborn/).

## Key Questions
- How do discounts impact revenue?
- What's the relationship between discount size and sales volume?
- Can we optimize discount strategy?

## Dataset
- `orderlines.csv` - Individual line items from orders
- `orders.csv` - Order-level metadata
- `products.csv` - Product catalog with pricing

## Data Quality Challenges
- 92% of orders contained discounts, making control group comparison impossible
- Discount data was corrupted and had to be reconstructed from price stamps

## Technologies
- Python 3.x
- Pandas (data manipulation)
- Seaborn (visualization)
- Google Sheets (presentation)

## Repository Structure
```
├── data/
│ ├── raw/ # Original CSV files
│ ├── cleaned/ # cl.csv files
│ └── quality/ # cu.csv files
├── notebooks/
│ ├── #_name_challenges.ipynb # Tutorial exercises
│ ├── #_name_solutions.ipynb # canonical solutions
│ ├── discount_analysis/ # My independent analysis
│ └── discount_analysis_seaborn/ # My independent analysis with plotting
├── presentation.pdf # Group presentation
└── README.md
```

## Key Findings
- Weak to no correlation between discount size and increased revenue
- Revenue used as primary KPI (profit data unrecoverable)
- Better effect of discounts in lower-priced segments
- No evidence of strategic discount campaigns - discounts appear ad-hoc

## Limitations
- Small sample size after data cleaning
- No profit margin data available
- Synthetic data may not reflect real-world patterns

## Future Work
- Implement proper discount tracking in database schema
- A/B testing framework for discount strategies
- Incorporate customer lifetime value metrics

## Author
Author: Niklas Livchitz — independent analysis in discount_analysis/ and discount_analysis_seaborn/
Group project: shared cleaning/exploration notebooks and the final presentation (presentation.pdf) were produced with bootcamp group collaborators.