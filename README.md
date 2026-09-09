# Collections & Delinquency Portfolio Analytics

A data analytics project analyzing a synthetic loan collections portfolio built to demonstrate delinquency tracking, recovery performance, and collector productivity analysis.

🔗 🔗 **[View the live dashboard](https://goldentoms.github.io/collections-delinquency-analytics_/Collections_Delinquency_Dashboard.html)**


Coming from a background in financial services collections and account management, I built this project to translate hands-on domain knowledge into an analytics deliverable — the kind of dashboard a collections operations team would actually use to prioritize accounts, monitor recovery performance, and evaluate collector productivity.

**Note:** All data in this project is synthetic, generated to resemble a realistic collections portfolio. No real customer or institutional data was used.

## Dataset

- 1,200 loan accounts across a 12-month tracking window (Sep 2025 – Aug 2026)
- Products: Personal Loan, Auto Loan, Credit Card, Line of Credit
- Regions: Ontario, Quebec, British Columbia, Alberta, Atlantic
- Fields: account ID, region, product, credit band, assigned collector, origination/outstanding balance, DPD bucket, days past due, contact attempts, promise-to-pay flag, amount recovered

## Key Findings

- **Overall delinquency rate: 32.7%** (392 of 1,200 accounts)
- **British Columbia** had the highest regional delinquency rate at 35.0%, vs. ~30% in Quebec, Alberta, and Atlantic
- **$7.18M total outstanding balance**, with **$578.5K recovered** from delinquent accounts to date
- **Recovery rate drops sharply as accounts age**: 61.5% in the 1-30 DPD bucket vs. 10.3% at 90+ DPD — reinforcing the value of early intervention
- **Collector performance varied meaningfully** in dollars recovered per account handled, pointing to a coaching/workload-rebalancing opportunity

## Repo Contents

| File | Description |
|---|---|
| `Collections_Delinquency_Dashboard.html` | Interactive dashboard (KPI tiles, delinquency trend, regional and collector breakdowns) — open directly in a browser |
| `Collections_Delinquency_Portfolio.xlsx` | Excel workbook with raw data + formula-driven summary dashboard (SUMIF/COUNTIF/AVERAGEIFS — no hardcoded values) |
| `collections_data.csv` | Underlying synthetic dataset |

## Tools Used

Python (pandas, numpy) for synthetic data generation · Excel (openpyxl) for the formula-driven workbook · HTML/CSS/Chart.js for the dashboard visualization

## Methodology

1. Generated a synthetic account-level dataset with realistic risk patterns by credit band and product type
2. Built an Excel workbook with a raw data tab and a fully formula-driven dashboard tab, so all KPIs recalculate automatically if the underlying data changes
3. Built a second, visual-first version of the dashboard for presentation, using the same underlying figures

## Contact

Open to feedback — feel free to reach out or connect on [LinkedIn](https://www.linkedin.com/in/ayomidetomoloju/).
