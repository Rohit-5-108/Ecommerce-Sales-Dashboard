# E-commerce Sales Dashboard | Power BI

An interactive Power BI dashboard designed to monitor e-commerce performance and explore sales and profitability across time, geography, product categories, sub-categories, and payment modes.

## Project Overview

This project brings key e-commerce metrics into one report so that users can quickly review overall performance and explore patterns in the underlying order data. The report uses the `Orders` and `Details` tables in its data model.

## Objectives

- Monitor overall sales amount, profit, quantity sold, and Average Order Value (AOV).
- Compare profit trends across months.
- Identify states contributing sales amount and sub-categories contributing profit.
- Understand the distribution of quantity by product category and payment mode.
- Present the information in a single, visually consistent report for faster exploration.

## Dashboard Contents

### KPI Cards

The report includes four KPI cards:

| KPI | What it represents |
|---|---|
| Sales Amount | Total of the `Amount` field |
| Profit | Total of the `Profit` field |
| Quantity Sold | Total of the `Quantity` field |
| Average Order Value (AOV) | AOV field displayed in the report; verify its aggregation before interpreting it as an average |

### Visualizations

1. **Monthly Profit Trend** — column chart showing profit by month based on `Order Date`.
2. **Profit by Sub-Category** — bar chart comparing sub-category profitability, sorted by profit.
3. **Quantity by Category** — donut chart showing the quantity distribution across product categories.
4. **Quantity by Payment Mode** — donut chart comparing quantity across payment modes.
5. **Sales Amount by State** — bar chart comparing sales amount across states.

## Tools and Technologies

- **Microsoft Power BI Desktop** — report creation and visualization
- **Power BI data model** — report fields from the `Orders` and `Details` tables
- **Data visualization and KPI reporting** — presenting and comparing business metrics

## How to Open the Project

1. Download or clone this repository.
2. Open `Ecommerce_Sales_Dashboard.pbix` using Microsoft Power BI Desktop.
3. If Power BI prompts for data-source credentials or a path, reconnect the required source and refresh the report.
4. Explore the KPI cards and charts to compare sales and profit across the report dimensions.

## Questions This Dashboard Helps Explore

- How does profit change from month to month?
- Which states have the highest sales amount?
- Which sub-categories contribute more or less profit?
- How is quantity distributed across product categories?
- Which payment modes account for larger shares of quantity?

The answers depend on the data loaded in the PBIX file; this README does not claim specific numeric findings.

## Repository Structure

```text
Ecommerce-Sales-Dashboard/
├── README.md
├── .gitignore
└── Ecommerce_Sales_Dashboard.pbix
```

## Notes Before Publishing

- **Check the AOV calculation:** Average Order Value is normally an average-based metric. Verify that the field is aggregated appropriately for your dataset rather than summed across rows.
- **Add dataset attribution:** The PBIX contains `Orders` and `Details` tables, but the original dataset source is not identified in the report metadata. If the data came from a tutorial, website, or another creator, add the source link and comply with its license before making the repository public.
- **Optional preview:** Export or capture the finished report in Power BI Desktop and add the image to the repository (for example, `screenshots/dashboard.png`) if you want a screenshot to appear on the GitHub page.

## Future Enhancements

- Add date, state, category, and payment-mode slicers where useful.
- Validate KPI definitions and create explicit DAX measures for consistent calculations.
- Add a report screenshot and a concise, data-backed findings section.
- Improve accessibility with descriptive titles, readable labels, and alt text for any repository screenshots.

---

**Project:** E-commerce Sales Dashboard  
**Built with:** Microsoft Power BI
