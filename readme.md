# Sales Analytics Dashboard

Analysis of 4 years (2015-2018) of Superstore sales data (9,800 orders) using Python for exploration/modeling and Power BI for a business-facing dashboard.

## Business Questions Answered
- What does the monthly sales trend look like, and is it seasonal?
- Which categories, sub-categories, and regions drive the most revenue?
- Can we forecast future monthly sales from historical data?

## Key Findings
- Sales are strongly seasonal: every year sees a sharp spike in Sep/Nov/Dec, with November 2018 ($117.9K) the highest single month in the dataset.
- Revenue is fairly balanced across categories — Technology ($827K), Furniture ($729K), Office Supplies ($705K) — no single category dominates.
- Phones and Chairs are the top 2 sub-categories by sales, each around $320K.
- West is the strongest region ($710K), South the weakest ($389K).
- A baseline linear regression model (time only) had a weak R² of 0.033. Adding calendar month as a feature to capture seasonality improved R² to 0.637 and cut prediction error (MAE) from $18.5K to $10.5K — showing seasonality, not linear growth, is the dominant driver of monthly sales.

## Tools Used
Python (Pandas, NumPy, Matplotlib, Seaborn, scikit-learn), Jupyter Notebook, Power BI

## How to Run
1. Clone this repo
2. `pip install -r requirements.txt`
3. Open `notebooks/01_exploration.ipynb` in Jupyter
4. Power BI dashboard: open `dashboard.pbix` in Power BI Desktop

## Dashboard Preview
![Power BI Dashboard](images/dashboard_powerbi.png)