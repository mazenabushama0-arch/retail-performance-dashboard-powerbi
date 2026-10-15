# Retail Performance Analytics (Power BI + Excel)

> 🌐 Part of my data analytics portfolio: [My-PORTFOLIO](https://mazenabushama0-arch.github.io/Portfolio/) · 👤 [More projects on my GitHub](https://github.com/mazenabushama0-arch)

A two-part retail analytics project for a multi-branch business:

- **Part 1 – Power BI report:** a multi-page report covering **sales, inventory, forecasting, store comparison, financials, and purchase orders**, with a home page and button navigation.
- **Part 2 – Excel dashboard:** an Excel workbook on a **Power Pivot data model** covering sales KPIs, inventory health, and like-for-like sales with a monthly forecast.

Together they turn raw sales, stock, and purchasing data into one view of branch, category, and vendor performance.

**Full preview (16 pages):** [`Retail_Performance_Analytics.pdf`](Retail_Performance_Analytics.pdf)

> **Data note:** Profit, margin, cost, salary, and bonus figures are blurred in the preview. In Part 2, all monetary amounts are blurred.

---

## Part 1 · Power BI report

| Page | What it answers |
|---|---|
| **Executive Dashboard** | Total sales, growth vs last year, sales by brand, region, and region manager, monthly trend vs last year, sold quantity by category |
| **Sales Performance** | MTD and YTD sales vs last year by store and category, with difference % |
| **Daily Performance** | Day-by-day sales with week-over-week (WoW %) and year-over-year (YoY %) comparison, plus sales by day of week |
| **Inventory** | On-hand units, model count, sell-through %, stock turn, stock by store and category, sell-through matrix (store × category) |
| **Stock To Sales** | Sell-through by store for a selected season and category, with Slow Moving stock flags |
| **Forecasting** | Next-month sales forecast by store and category, driven by a selectable growth % |
| **AI Insights** | Key-influencers analysis showing what drives changes in total sales |
| **Comparison** | Current vs previous period by store: quantity, sales, margin, transactions, and growth % |
| **Purchase Orders** | Ordered vs received quantity, fulfillment rate by vendor, and open PO value by category and store |
| **Financial** | Daily sales vs expenses, expense breakdown by category and store, and net profit tracking |

**Key measures:** Sales MTD / YTD and last-year equivalents · MTD / YTD Diff % · WoW % and YoY % · Sell-Through % · Stock Turn · Slow Moving status · Forecast Sales (last year's next-month sales × selected growth %) · Fulfillment Rate % · Open PO %

---

## Part 2 · Excel dashboard

| Page | What it shows |
|---|---|
| **KPI – Sales** | Quantity, sales, ATV, and UPT; monthly sales trend; quarter view; top 10 stores; sales by category; size chart |
| **Inventory Executive Dashboard** | Warehouse and store stock, low-stock and active SKUs, inventory value by branch, category, vendor, and season, old-season share |
| **Sales Executive – LFL & Forecast** | Like-for-like sales MTD and YTD vs last year, store ranking by YoY growth, monthly forecast by store and category |
| **Data Model** | Relationships between Sales, Inventory, Vouchers, and Transfers and the shared dimensions (store, brand, category, season, date) |

**Interactivity:** slicers for year, quarter, month, store, and vendor.

---

## Tech stack

- **Power BI Desktop**: DAX measures and time-intelligence, Power Query for cleaning and transformation
- **Microsoft Excel**: Power Pivot data model, DAX, slicers
- **SQL / Excel** as data sources

---

## How it works

1. **Data prep:** clean and standardize sales, stock, and purchase-order tables; fix naming for stores, brands, and categories.
2. **Data model:** fact tables (sales, inventory, vouchers, transfers, purchase orders, expenses) connected to shared dimensions (store, brand, category, season, date).
3. **Measures (DAX):** MTD, YTD, and last-year comparison; sell-through, stock turn, and forecast logic.
4. **Report design:** consistent slicers, KPI cards on top, drill-down visuals below, button navigation between pages.

---

<!-- Add screenshots to an /images folder, then uncomment:
## Screenshots
![Power BI – Executive Dashboard](images/powerbi-executive.png)
![Power BI – Inventory](images/powerbi-inventory.png)
![Excel – KPI Sales](images/excel-kpi-sales.png)
![Excel – Inventory](images/excel-inventory.png)
-->

## Author

**Mazen Mohsen**
Senior Data & Merchandise Analyst
[LinkedIn](https://linkedin.com/in/mazen-abushama-934246398)
