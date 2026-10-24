# Regional Sales Analysis Dashboard (Excel)

An Excel workbook that analyses sales performance across three Kenyan regions (Nairobi, Mombasa, Kisumu) and three product categories (Beverages, Household, Snacks), using PivotTables, charts, and an interactive Region slicer.

## Short Description

> An Excel sales analysis project that summarises revenue, units sold, and customer ratings by region and product category, with PivotTables, a pie chart, a bar chart, and a Region slicer for interactive filtering.

## What's Inside

| Sheet | Contents |
|-------|----------|
| `Sheet1` | **Raw data table** (12 records, January–April) |
| `Sheet2` | PivotTable: Revenue (Ksh) by Region (rows) and Product Category (columns), titled "Revenue (Ksh) by Region and Product Category" |
| `Sheet3` | PivotTable: Revenue by Product Category, with a **pie chart** showing each category's share of total revenue |
| `Sheet7` | PivotTable: Revenue by Product Category, with a **bar chart**; this one is connected to the **Region slicer** (currently filtered to Nairobi) |
| `Sheet8` | A second copy of the Region × Category revenue PivotTable |

## Dataset

| Column | Description |
|--------|-------------|
| `Month` | Month of the sale (January–April) |
| `Region` | Nairobi, Mombasa, or Kisumu |
| `Product Category` | Beverages, Household, or Snacks |
| `Units Sold` | Number of units sold |
| `Revenue (Ksh)` | Revenue in Kenya Shillings |
| `Customer Rating` | Average customer rating (out of 5) |

## Key Findings

Calculated from the raw data in `Sheet1`:

- **Total revenue:** Ksh 672,500 from 1,185 units sold
- **Top region:** Nairobi leads with Ksh 274,500 (500 units) and also the highest average rating (4.30)
- **Top category:** Household brings in the most revenue (Ksh 279,000), followed by Beverages (Ksh 217,500) and Snacks (Ksh 176,000)
- **Mombasa vs Kisumu:** these two are close in revenue (Ksh 198,000 vs Ksh 200,000), but Mombasa sells more units (385 vs 300), so Kisumu earns more per unit
- **Best months:** March (Ksh 202,500) and April (Ksh 201,500) are far ahead of January (Ksh 142,500) and February (Ksh 126,000)
- **Customer satisfaction:** the overall average rating is 4.03, with Nairobi highest and Kisumu lowest (3.88)

## How to Use

1. Open `Book1.xlsx` in Microsoft Excel (PivotTables and slicers work best in Excel 2013 or later)
2. Go to `Sheet7` and click a region on the **Region slicer** to filter the bar chart and table
3. To add new data, append rows to the table in `Sheet1`, then go to **Data → Refresh All** so the PivotTables and charts update

## Known Issue

The PivotTables currently show a total of **Ksh 672,000**, while the raw data adds up to **Ksh 672,500**. The Nairobi Household figure in the PivotTables is 85,000, but the raw data has 85,500 for March. This means the PivotTables were not refreshed after that cell was edited. Click **Data → Refresh All** to fix it (Household should then show 279,000 and Nairobi 274,500).

## Tools Used

- Microsoft Excel: PivotTables, PivotCharts, Slicers, Tables

## Possible Improvements

- Rename sheets descriptively (e.g. `Raw Data`, `Revenue by Region`, `Category Share`)
- Remove the duplicate PivotTable in `Sheet8`
- Add a calculated revenue-per-unit column
- Add a month-over-month revenue trend chart
- Extend the data beyond April to analyse seasonality
- Add a Month slicer alongside the Region slicer

## License

This project is open for learning and educational use.
