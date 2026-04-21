# ACC102 Track2: Tech Giants Financial Analysis (2019-2024)

## Project Overview
This project analyzes the financial performance of four major U.S. technology companies (Apple, Microsoft, Google, and Amazon) from 2019 to 2024. Using data from the WRDS Compustat database, we examine trends in revenue, net income, return on equity (ROE), and gross margin.

## Data Source
- **Database**: WRDS Compustat (Fundamentals Annual - funda)
- **Sample**: AAPL, MSFT, GOOGL, AMZN
- **Period**: 2019–2024
- **Key Variables**: Total Revenue (revt), Net Income (ni), Gross Profit (gp), Sales (sale), Shareholder's Equity (seq), Total Assets (at)

## Methodology
1.  **Data Extraction**: Connect to WRDS and pull annual financial statements.
2.  **Data Cleaning**: Remove missing values and standardize units (convert to billions USD).
3.  **Ratio Calculation**:
    - ROE = (Net Income / Shareholder's Equity) × 100
    - Gross Margin = (Gross Profit / Sales) × 100
4.  **Analysis & Visualization**:
    - Create pivot tables for year-over-year comparison
    - Plot trends in revenue, net income, ROE, and gross margin using Matplotlib
5.  **Export Results**: Save cleaned data, pivot tables, and plots for review.

## Key Findings
- **Revenue Growth**: All four companies showed consistent revenue growth over the period, with Apple and Amazon leading in total revenue.
- **Profitability**: Microsoft maintained the highest and most stable ROE, reflecting strong shareholder returns.
- **Margins**: Google and Apple consistently maintained high gross margins, while Amazon's margins improved over time.
- **Resilience**: All firms demonstrated strong financial recovery and growth post-2020.

## Files in This Repository
- `Tech Giants Financial Analysis.ipynb`: Full Python code and analysis
- `financial_analysis.png`: Summary plot of all four metrics
- `tech_giants_financial_data.csv`: Cleaned raw financial data
- `revenue_pivot.csv`: Pivot table of revenue by company and year
- `roe_pivot.csv`: Pivot table of ROE by company and year
- `.gitignore`: Python project ignore rules

## How to Run
1.  Install required packages: `pip install wrds pandas matplotlib`
2.  Open `Tech Giants Financial Analysis.ipynb` in Jupyter Notebook
3.  Run the code and enter your WRDS credentials when prompted

## Limitations & Future Work
- The analysis is limited to annual data; quarterly data could provide more granular insights.
- The sample size is small; future work could expand to more companies or industries.
- Additional metrics like debt ratios or price-to-earnings ratios could be added for a more complete picture.
