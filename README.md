# SuperStore Sales & Profitability Analysis

Exploratory data analysis of 9,994 retail order lines (2014-2017) to find where the business makes and loses money.

**Tools:** Python, pandas, matplotlib, Jupyter

## Key findings
- Sales of **$2.30M** and profit of **$286K** (12.5% margin), yet **18.7%** of order lines lose money.
- **Discounting drives the losses:** orders discounted above 20% were unprofitable **97%** of the time (1,393 lines, -$135K combined). Undiscounted orders earn a 29.5% margin; discounts of 61%+ lose 122% of sales.
- **Tables, Bookcases and Supplies are loss-making.** Tables alone lose $17.7K (-8.6% margin).
- **Central region margin is 7.9%** versus 14.9% in West. Texas, Ohio, Pennsylvania and Illinois are the largest loss-making states.
- Furniture earns a 2.5% margin versus 17% for Office Supplies and Technology.

## Recommendations
- Cap discounts at 20% and require approval above that level.
- Review pricing and discounting on Tables and Bookcases.
- Investigate discount-heavy accounts in the Central region and the loss-making states.

## Charts
![Profit by sub-category](images/profit_by_subcategory.png)
![Margin by discount band](images/margin_by_discount.png)
![Least profitable states](images/worst_states.png)

## Run it
```bash
pip install pandas matplotlib jupyter
jupyter notebook superstore_analysis.ipynb
```
Dataset: Sample - Superstore (public sample dataset), included in `data/`.
