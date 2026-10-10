# Cafe Sales Data Analysis

A data analysis project built in Excel to explore sales patterns for a simulated four-branch Metro Manila cafe across calendar year 2025.

**Status:** Completed using simulated point-of-sale data  
**Dashboard:** [`dashboard/`](dashboard/) (includes the Excel workbook)  
**Raw data:** [`dashboard/raw_data.csv`](dashboard/raw_data.csv) (1,836 rows)  
**Source workbook:** [Open Cafe_Sales_Data_Analysis.xlsx in Excel for the web](https://1drv.ms/x/c/069d45d704321105/IQB7gz0k0iGoSpKTa5mOP4mzAbgmGbr9GE1wf-WhUz9EFN4?e=Fj6fjm)

## Project question

Where does a four-branch Metro Manila cafe make its money, and how can its sales patterns inform revenue-growth decisions?

## Data and scope

The workbook uses a **simulated point-of-sale export** for 2025. Each row represents one product line on an order. Fields include order ID, date, hour, branch, product and category, quantity, unit price, discount, payment method, and customer type.

The raw data intentionally includes duplicates, typos, blanks, text-formatted dates, and outliers so the cleaning process can be demonstrated. It does not represent real business transactions.

The repository's [`raw_data.csv`](dashboard/raw_data.csv) is an uncleaned export of the workbook's `1_Raw_Data` sheet. It contains simulated data only and is published so the raw inputs can be viewed directly on GitHub.

## Repository layout

- [`analysis/`](analysis/) contains the workbook's interpretation, recommendations, and limitations.
- [`charts/`](charts/) contains image exports of all eight workbook charts.
- [`dashboard/`](dashboard/) contains the Excel workbook, browser dashboard, and raw CSV.

## Analysis workflow

1. Preserve the untouched raw export.
2. Inspect blanks, duplicates, text values, invalid numbers, and inconsistent labels.
3. Document cleaning decisions and prepare a separate clean dataset.
4. Calculate net revenue, average order value, discount rate, median, spread, and units per order.
5. Group results by branch, category, product, month, weekday, time slot, hour, payment method, and customer type.
6. Compare branches, weekdays and weekends, discounted and full-price sales, and seasonal/category patterns.
7. Create eight charts linked to the analysis tables.
8. Interpret eight findings with supporting evidence.
9. Propose eight prioritized actions with success measures.

## Workbook highlights

- **Net revenue:** ₱394,428 (workbook headline result)
- **Coverage:** 4 branches across calendar year 2025
- **Visualizations:** 8 charts in the workbook
- **Workbook structure:** README, raw data, inspection, cleaning log, clean data, calculations, grouping, comparisons, visualizations, interpretations, and recommendations

All headline values describe the simulated workbook data, not a real cafe.

## Project files

```text
cafe-sales-data-analysis/
├── README.md
├── analysis/
│   └── README.md
├── charts/
│   ├── README.md
│   ├── index.html
│   ├── *.svg
│   └── *.png
└── dashboard/
    ├── README.md
    ├── index.html
    ├── Cafe_Sales_Data_Analysis.xlsx
    └── raw_data.csv
```

The repository dashboard summarizes the project and links to the raw dataset and full Excel workbook, which contains the cleaned data, formulas, charts, findings, and recommendations.

## Tools

- Microsoft Excel
- Data inspection, cleaning, formulas, grouping, comparison, and charting
- Git and GitHub for project documentation and version control

## Reproducibility and privacy

The source workbook is shared through OneDrive. Its raw and cleaned sheets are kept separate, and the cleaning log records the transformations. Do not replace the simulated data with private business or customer data unless you have authorization and have removed sensitive information.
