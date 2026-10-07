# Retail Performance Dashboard (Power BI)

A multi-page Power BI report that brings retail **sales, inventory, forecasting, store comparison, financials, and purchase orders** into one navigable dashboard, with a home page and button navigation between pages.

> **Data note:** Sensitive figures (profit, margin, cost, salaries, bonuses) are blurred in the PDF and screenshots in this repo. Nothing here is a confidential data source.

---

## Dashboard pages

| Page | What it answers |
|---|---|
| **Home / Navigation** | Landing page with buttons to every report page |
| **Executive Dashboard** | Total sales, YTD vs last year, growth %, sales by brand, region, and region manager, monthly trend vs last year, sold quantity by category |
| **Sales Performance** | MTD and YTD sales vs last year by store and by category, with MTD and YTD difference % |
| **Daily Performance** | Day-by-day sales with week-over-week (WoW %) and year-over-year (YoY %) comparison, plus sales by day of week |
| **Inventory** | On-hand units, model count, sell-through %, stock turn, stock by store and category, sell-through matrix (store × category) |
| **Stock To Sales** | Sell-through by store for a selected season and category, with Slow Moving stock status flags |
| **Forecasting** | Next-month sales forecast by store and category, driven by a selectable growth % |
| **AI Insights** | Key-influencers analysis showing what drives changes in total sales |
| **Comparison** | Current vs previous period by store: quantity, sales, profit, margin, transactions, and growth % |
| **Financial** | Daily sales vs expenses, expense breakdown by category and store, and net profit tracking |
| **Purchase Orders** | Ordered vs received quantity, PO cost, fulfillment rate by vendor, and open PO value by category and store |

---

## Key measures

- **Sales MTD / YTD** and their last-year equivalents, with **MTD Diff %** and **YTD Diff %**
- **WoW %** and **YoY %** for daily trend analysis
- **Sell-Through %** (units sold relative to units received) and **Stock Turn**
- **Slow Moving** status based on sell-through thresholds
- **Forecast Sales** = last year's next-month sales × selected growth %
- **Fulfillment Rate %** and **Open PO %** for purchasing

---

## Tech stack

- **Power BI Desktop**
- **DAX** for measures and time-intelligence
- **Power Query** for data cleaning and transformation
- **SQL / Excel** as data sources

---

## Screenshots

Add your images to an `/images` folder and link them here:

```
![Executive Dashboard](images/01-executive.png)
![Daily Performance](images/02-daily.png)
![Inventory](images/03-inventory.png)
![Forecasting](images/04-forecasting.png)
![Stock To Sales](images/05-stock-to-sales.png)
![Comparison](images/06-comparison.png)
![Purchase Orders](images/07-purchase-orders.png)
```

Full report preview: [`Sales_Analysis_blurred.pdf`](Sales_Analysis_blurred.pdf)

---

## How the model works

1. **Data prep (Power Query):** clean and standardize sales, stock, and PO tables; remove duplicates and fix naming for stores, brands, and categories.
2. **Data model:** star schema with fact tables (sales, stock, purchase orders, expenses) connected to shared dimensions (store, product/category, calendar).
3. **Measures (DAX):** time-intelligence for MTD, YTD, and last-year comparison; sell-through, stock turn, and forecast logic.
4. **Report design:** consistent slicers (year, month, store, category, brand), KPI cards on top, drill-down visuals below, button navigation between pages.

---

## Author

**Mazen Mohsen**
Senior Data & Merchandise Analyst
[LinkedIn](https://linkedin.com/in/mazen-abushama-934246398)
