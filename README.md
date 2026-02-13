# Gameszone-sales-performance-dashboard-excel-tableau
End-to-end sales performance analysis and interactive Tableau dashboard for a retail gaming company, built using Excel for cleaning and Tableau for business insights.Retail sales performance dashboard analyzing products, regions, channels, AOV, YoY growth, and refunds using Tableau.
## Sales Performance Dashboard (Overview)

The dashboard below provides an executive view of **sales performance across products, regions, and marketing channels** for the period **Jan 2019 – Feb 2021**.  
It consolidates ~**21k transactions** into decision-ready KPIs and diagnostic visuals to support marketing, operations, and category management decisions.

**How to read this dashboard**
- **Top KPIs:** Total Sales, Average Order Value (AOV), YoY Sales Growth, Total Orders  
- **Filters:** Product, Region, Marketing Channel, Month  
- **Core Views:** Product sales trends, sales mix by product, refunds by product, regional revenue, channel performance, and product-level tables (sales, AOV, orders)

**What this helps decide**
- Which products and regions to prioritize for inventory and promotions  
- Which channels to scale or diversify to reduce revenue concentration risk  
- Where refunds are concentrated and which SKUs need operational fixes  
- When seasonal peaks occur to plan campaigns and stock


<!-- Main Sales Performance Dashboard (Full view) -->
![Sales Performance Dashboard – Full View](https://github.com/ronaksinghconnect/Gameszone-sales-performance-dashboard-excel-tableau/blob/main/FINAL%20Sales%20Performance%20dashboard.png)
# Games Zone — Sales Performance Dashboard (End-to-end Project)

## Project summary (one-line)
Built an end-to-end sales performance dashboard for **Games Zone** from raw transaction data (≈21k rows) — cleaning and feature engineering in Excel, deep-dive analysis and final interactive visuals in Tableau — producing executive KPIs, product & channel diagnostics, and actionable recommendations for marketing, operations and category teams.

---

## Problem statement
Games Zone had fragmented, noisy transactional data and no single place for leadership to quickly answer business-critical questions such as:
- Where is revenue coming from (products, channels, regions)?  
- Which products and categories drive revenue and returns?  
- When are peak months and how does seasonality affect AOV and channel mix?  
- Which operational issues (returns, refunds) are leaking revenue?

Leadership needed a consolidated, decision-ready view that replaced manual spreadsheet exploration with fast, repeatable insight.

---
## What I delivered (high-level)
- A single-page **Sales Performance Dashboard** in Tableau with interactive filters (Product, Region, Channel, Month).  
- Executive KPI bar at the top: **Total sales, Average Order Value (AOV), YoY% sales, Total orders** for quick executive decisions.  
- Deep visuals for product-level trends, refund dynamics, regional performance, and sales mix.  
- A documented data-cleaning & issue log (Excel) that records every fix, its rationale, row counts affected and resolution — enabling auditability and reproducibility.  
- Clear, prioritized recommendations for Marketing, Operations, Category and Supply Planning teams.

---
## Solution overview — Key metrics (executive snapshot)
(The numbers below are displayed on the top of the Tableau dashboard and are calculated across the dataset unless filtered.)

- **Total sales:** **$6,151K**  
- **Average Order Value (AOV):** **$283.23**  
- **Year-over-Year (YoY) Sales Growth:** **164.27%** (shows rapid growth during 2020)  
- **Total orders:** **21,863**  
- **Total refunds (count):** **~3,487** (aggregate across products/time)  
- **Top revenue product:** **27in 4K gaming monitor** — **$1,969K** revenue, **4,723** orders  
- **2nd / 3rd top products:** **Nintendo Switch** — **$1,659K** (10,386 orders), **Sony PlayStation 5 Bundle** — **$1,589K** (977 orders)  
- **Top 5 products** together account for a large share of total revenue (the dataset is product-concentrated).  
- **Refund concentration:** Nintendo Switch and 27in monitor are among products with highest refund counts (significant operational leakage to investigate).  
- **Regional mix (approx):** North America ~40–50%, EMEA ~25–35%, APAC ~8–12% (stacked monthly revenue shows NA largest contributor)  
- **Channel mix:** Top channel ≈ **35%** of revenue (Direct or a marketplace, depending on filter), next two channels ≈ **22–23% each** — indicates concentration risk. ----
## Dataset & scope
- **Dataset name:** Games Zone — Sales transactions (internal/sample dataset)  
- **Row count:** ~21,000 order-level transactions (21k)  
- **Time range:** Jan 2019 – Feb 2021 (monthly granularity used in visuals)  
- **Key fields used:** Order date, Product name, Unit price / sales, Quantity, Channel (direct/email/affiliate/social), Region, Order status, Customer-related fields (used to derive segments)  
- **Tools:** Microsoft Excel (cleaning, feature engineering, pivot checks), Tableau (dashboard & visuals)

## Exploratory Insights (Excel)

Before building dashboards in Tableau, I conducted high-level exploratory analysis in Excel to understand overall revenue trends and product performance (time range: Jan 2019 – Feb 2021).

### Key exploratory findings
- **Overall revenue trend:**  
  Total annual revenue increased from 2019 to 2020 (approx. $6.1M in 2020), with monthly sales growing from ~$100K in early 2019 to peaks above ~$550K during late 2020.

- **Top-performing product:**  
  The **27in 4K gaming monitor** emerged as the highest revenue contributor (~$1.96M), indicating strong demand for premium hardware.

- **Low-performing products:**  
  Accessories such as **gaming headsets** and **gaming mice** contributed a very small share (~2%) of total revenue, suggesting underperformance or low-margin volume sales.

- **Product growth patterns:**  
  Most products performed better in 2020 compared to 2019, indicating strong year-over-year growth across the portfolio.

- **Stagnant growth signals:**  
  Certain products (e.g., JBL Quantum headset) showed relatively flat growth compared to other SKUs, highlighting candidates for repositioning, bundling, or pricing strategy review.

> **Context note:**  
> Observed trends in 2020 may be influenced by external factors such as COVID-19, which likely altered customer behavior and demand patterns.  
> The analysis focuses on internal performance signals and assumes no major external shocks; results should be interpreted with this limitation in mind.
---
## Deep-Dive Insights & Recommendations (Tableau)

Beyond high-level KPIs, I created multiple analytical views in Tableau to connect **observations directly to business actions** across teams.

### Refund Analysis (by Product)
**Finding:**  
Nintendo Switch recorded the highest number of refunds, followed by the 27in 4K gaming monitor.

**Recommendation (Product & Operations):**  
- Investigate root causes behind high refund rates (product defects, delivery issues, mismatched expectations).  
- Strengthen product QA and improve product detail pages to reduce preventable returns.

---

### Channel Performance (Sales by Channel)
**Finding:**  
The **Direct channel** drove the highest total sales across top products, with **Email** as the second-largest contributor.

**Recommendation (Marketing):**  
- Scale high-performing Direct and Email campaigns using better segmentation and lifecycle targeting.  
- Run controlled experiments on Social and Affiliate channels to diversify acquisition and reduce channel concentration risk.

---

### Regional & Channel Trends
**Finding:**  
Sales dips for products like **Sony PlayStation 5** from Dec 2020 to Jan 2021 were primarily driven by declines in **North America and EMEA via the Direct channel**.

**Recommendation (Regional Ops & Supply Chain):**  
- Launch region-specific recovery campaigns in NA and EMEA for high-demand products.  
- Align inventory planning with regional demand to prevent stockouts amplifying seasonal dips.

---

### Seasonal Channel Volatility
**Finding:**  
The Direct channel experienced a notable dip from Dec 2019 to Jan 2020 for products such as gaming monitors and Nintendo Switch, followed by a strong spike in Dec 2020.

**Recommendation (Performance Marketing):**  
- Audit Direct channel funnel friction during year-end transitions (checkout flow, promo timing).  
- Codify successful Dec 2020 campaign strategies (offers, creatives, landing pages) into a repeatable peak-season playbook.

---

### Average Order Value (AOV) by Product
**Finding:**  
High-ticket products (e.g., PS5 bundles, gaming laptops) have significantly higher AOV, while high-volume products (e.g., Nintendo Switch) generate lower AOV despite high order counts.

**Recommendation (Sales & Growth):**  
- Focus premium bundles and campaigns around high-AOV products to maximize revenue per transaction.  
- Increase AOV for lower-priced products via cross-sell bundles and “buy more, save more” offers.

---

### YoY Growth & Campaign Timing
**Finding:**  
Strong YoY growth spikes (e.g., ~4x revenue growth for PS5 bundles during peak months) indicate the impact of successful product/channel pushes.

**Recommendation (Growth & Marketing):**  
- Double down on high-growth products during peak demand windows.  
- Replicate winning promotion strategies (timing, messaging, channel mix) across other high-potential SKUs to scale growth.
## Analytical Workflow (From Raw Data to Business Decisions)

1. **Initial exploration (Excel)**
   - Quick pivot tables to check distribution by month, product, region and channel.
   - Visual checks for missing/odd values.

2. **Data cleaning & logging (Excel)**
   - Created an issue log with row counts and resolutions (every change auditable).
   - Standardized product names, region codes, channel values.
   - Fixed inconsistent gender & demographic values where present.
   - Converted numeric-like strings and worded quantities (e.g., “one”, “two”) to integers.
   - Resolved date formatting issues and confirmed all order dates parse correctly.
   - Removed/flagged duplicates; preserved raw backup before destructive ops.

3. **Feature engineering (Excel)**
   - Extracted `Month` and `MonthStart` for consistent time axis in Tableau.
   - Built `Age Group` and other segments where demographic fields were available.
   - Calculated `First purchase date` per customer and a `New vs Existing` flag for lifecycle analysis.
   - Calculated `Refund flag` and `Refunded sales` for refund-focused metrics.

4. **Validation**
   - Reconciled aggregate totals (Excel pivots) vs Tableau extracts to ensure parity.
   - Performed sanity checks (AOV = Total sales / Total orders, refund rate, etc.)

5. **Dashboard design (Tableau)**
   - Executive KPI row (Total sales / AOV / YoY / Orders) with small trend sparklines beneath each KPI.
   - Multi-chart canvas: product trend lines, stacked sales mix, refund trend & mix, product-level tables (sales / AOV / count), regional stacked columns, and interactive filters (Product / Region / Channel / Month).
   - Designed charts to directly map to stakeholder questions (no decorative charts).

6. **Interpretation & action**
   - Turned quantitative findings into concrete recommendations for Marketing, Ops, Category and Supply Planning teams.

---

## Data Validation & Quality Assurance
To ensure metric accuracy and trustworthiness:
- Reconciled Tableau aggregates against Excel pivot totals for Total Sales, Orders, and AOV.  
- Performed sanity checks on KPI formulas (e.g., AOV = Total Sales / Total Orders).  
- Spot-checked monthly revenue totals against raw transaction sums.  
- Logged all data issues and resolutions in a dedicated cleaning log to maintain auditability.
 
---

## Detailed dashboard insights (chart-by-chart, with numbers & business meaning)

### 1) Executive KPIs & trends
- **Total sales = $6,151K** with a clear upward trend during 2020 and a peak around Nov–Dec 2020.  
- **AOV = $283.23**, relatively stable with upward drift in late 2020 — suggests increase in basket/unit price (either higher-priced products or fewer discounts).  
- **YoY Sales = 164.27%** — strong growth year-on-year, likely driven by product launches, channel performance and pandemic purchasing patterns.

**Business meaning:** strong revenue growth, but seasonal concentration and AOV behaviour require channel- and campaign-level ROI checks.

---

### 2) Product-level trends (Sales products)
- **27in 4K monitor** leads revenue (~$1.97M) with **4,723** orders.  
- **Nintendo Switch** shows highest order count (~10,386) but lower AOV vs monitor. Total sales ≈ **$1.66M**.  
- **PS5 bundle** revenue ≈ **$1.59M** from **977** orders — very high AOV (~$1,643 per order for PS5 in the product table), indicating premium item behaviour.  
- Large seasonal spikes for top products in late 2020 — coordinate inventory and marketing for these periods.

**Business meaning:** product portfolio has both high-volume mid-priced items (Switch) and high-ticket drivers (Monitor, PS5). Inventory and promotion planning should reflect these different dynamics.

---

### 3) Count of orders (trend)
- Total orders ~**21,863**.  
- Product order counts show strong monthly growth in 2020, with notable spikes at year-end.

**Business meaning:** marketing and fulfillment must be scaled for peak months. Also monitor AOV vs count: months with rising counts but falling AOV indicate discount-heavy activity.

---

### 4) Refunds by product & refund mix
- **Total refund events ≈ 3,487**.  
- Refunds concentrate heavily in a few products (Nintendo Switch and 27in monitor among the top refund contributors). Example counts from the refund table: **Nintendo Switch refunds ~2,012**, **27in monitor refunds ~978** (refunded sales figures also shown in the refund table view).  
- Refund counts spike in mid-to-late 2020.

**Business meaning & recommendation:** high refunds on high-volume or high-value items are urgent. Root-cause analysis recommended: product defects, incorrect listings, or fulfillment errors. Tighten QA, update product pages (size/specs), and track refund root causes by product.

---

### 5) Sales mix & stacked area (by product)
- Stacked area reveals product mix dynamics across months: the top few products consistently make up the largest area share, but relative contributions shift during peak months.

**Business meaning:** leverage high-share products for cross-sell and bundle strategies, and test promotions on mid-tier products to spread risk.

---

### 6) Regional revenue (stacked columns)
- Monthly stacked columns show **North America** as the dominant region, followed by **EMEA** and **APAC**. A large surge in total monthly revenue occurs in mid-2020 across all regions, with NA contributing the largest absolute increase (seen as green bars in stacked chart).  
- Example month peaks: one month reaches >$500K in revenue (stacked across regions).

**Business meaning:** resource allocation (marketing, logistics) should prioritize NA and EMEA where volumes and margins are highest; explore targeted experiments in APAC or LATAM to diversify growth.

---

### 7) Regional trends by channel & product (small multiples)
- The dashboard includes rows of product-by-region trend panes (e.g., 27in monitor, Nintendo Switch, PS5) that reveal channel-specific performance per region.  
- Some products show strong regional seasonality (e.g., PS5 and gaming monitors spike strongly in NA/EMEA in late 2020).

**Business meaning:** regional promotions and localized inventory planning will maximize revenue capture and avoid stockouts during peaks.

---

### 8) Sales table (product-level KPIs)
- Product table shows **sales**, **AOV**, and **order counts** for direct comparison: e.g., PS5 high AOV (~$1,643) vs Nintendo Switch lower AOV (~$161) but very high order count.  
- Use this table for prioritizing category managers’ action plans.

---

## Data Cleaning in Excel (Issue Log & Resolutions)

All data quality issues identified during exploration were logged in Excel along with their row-level impact, resolution status, and treatment decision.  
Wherever a correction or recategorization was required, the cleaned value was written to a **new column** to preserve the original raw data for traceability.

### Summary of Data Quality Issues Addressed

- **Inconsistent date formats (purchase_ts):**  
  Detected mixed date formats across ~10 rows (~0.05% of data).  
  → Recategorized into a standardized date format to enable correct time-series analysis.

- **Blank / null timestamps (purchase_ts, refund_ts):**  
  A small number of records contained missing timestamps (≈1–37 rows, <0.2%).  
  → Left as-is and excluded from time-based aggregations where necessary to avoid introducing bias.

- **Product name inconsistencies:**  
  Identified spelling variations for key SKUs (e.g., “27in 4K gaming monitor”) across ~61 rows (~0.28%).  
  → Recategorized into a single standardized product name to ensure accurate product-level aggregation.

- **Null and zero values in price fields (usd_price):**  
  Detected nulls (~5 rows) and zero values (~29 rows, ~0.13%).  
  → Left unchanged but flagged, as zero-price transactions may represent promotions, test orders, or data capture issues.

- **Unknown and blank marketing channels:**  
  Found ~130 rows (~0.6%) with missing or blank channel values.  
  → Recategorized blanks as “Unknown” to preserve records while keeping channel segmentation consistent.

- **Unknown / blank account creation method:**  
  Identified ~826 rows (~3.8%) with missing values.  
  → Recategorized blanks to “Unknown” for consistency in customer segmentation analysis.

- **Region inconsistencies and blanks:**  
  Corrected region labels using country codes where available.  
  → Left truly unknown regions as-is but ensured EU/APAC country codes mapped to the correct regions.

- **Duplicate order IDs:**  
  Identified ~80 duplicate rows (~0.37%).  
  → Flagged and left unchanged in the working table (raw data preserved); duplicates were excluded from KPI calculations in Tableau where appropriate.

- **Shipping dates before purchase dates:**  
  Detected ~2,005 rows (~9.17%) where shipping date preceded purchase date.  
  → Flagged as data quality issues and excluded from delivery-time analyses, as these likely reflect system logging errors.

### Data Integrity Principles Followed

- Raw data was preserved and never overwritten.  
- All transformations were applied to **new cleaned columns** to maintain lineage and auditability.  
- Edge cases (nulls, zeros, unknowns) were retained unless they materially broke KPI logic.  
- Cleaning decisions were documented with row counts and rationale to support reproducibility and review.
- **Reconciled duplicates** (kept original backup, removed obvious duplicates).  
- **Mapped region codes** and filled obvious blanks where possible; left ambiguous nulls as-is but flagged.  
- **Engineered features**: MonthStart, AgeGroup, FirstPurchaseDate, New/Existing flag, RefundFlag, RefundedSales.

(Technical cleaning steps, exact formulas and row counts are stored in `data_cleaning_log.xlsx` in the repo.)

---

## KPIs tracked
- Total sales (USD)  
- Total orders (count)  
- Average Order Value (AOV = Total sales / Total orders)  
- Refund count & refunded sales (by product/channel/region)  
- Orders by product, channel, region, and age group  
- Monthly YoY% sales growth  
- Top product contribution (% of total sales)

---

## Decision use-cases (how teams will use this dashboard)
- **Marketing:** identify peak months and high-value segments to prioritize campaign spend; replicate high-performing channel creatives during peaks.  
- **Operations / Fulfillment:** identify products with high refunds to prioritize QA, returns processing and SKU-level fulfillment checks.  
- **Sales / Commercial:** focus seller incentives or vendor negotiations on top-performing product categories and channels.  
- **Category & Inventory Managers:** prioritize stock for high-revenue, high-margin products and plan replenishment for peak months.

---

## Limitations & next steps
**Limitations**
- Dataset is transactional only — lacks marketing spend, cost-of-goods sold (COGS), and customer lifetime values (CLV).  
- Some ‘region’ and ‘channel’ values contain nulls that limit perfect reconciliation.  
- Refund root causes are not directly available (need returns reason codes).

**Next steps**
- Add CLV/cohort analysis with customer IDs and RFM to guide retention strategy.  
- Combine marketing spend data to compute channel ROI and CAC.  
- Drill into returns: add reason codes and time-to-return to prioritize product fixes.  
- Build an operational alerting dashboard for refund rate spikes and inventory stockouts.
 
## Example Business Decisions Enabled
- Marketing can reallocate budget toward high-performing channels during peak months identified in the dashboard.  
- Operations can prioritize QA improvements for products with the highest refund counts to reduce revenue leakage.  
- Category managers can increase inventory coverage for high-velocity products ahead of seasonal spikes.  
- Leadership can monitor revenue concentration risk and set targets to diversify channel contribution.
---

## Files included in the repository
- `README.md` (this file)  
- `games_zone_transactions_cleaned.csv` (cleaned dataset used for dashboards) containing 
  `data_cleaning_log.xlsx` (issue log, row counts, and detailed resolutions)  
- `GamesZone_Sales_Performance.twbx` (Tableau packaged workbook with dashboards)  
- `screenshots/` (key images used in the portfolio README)  


---

## Reproducibility & how to run
1. Open `games_zone_transactions_cleaned.csv` in Excel to review cleaned source.  
2. Open `GamesZone_Sales_Performance.twbx` in Tableau Desktop (or Tableau Reader) — filters and dashboards will work out-of-the-box because workbook is packaged.  
3. To reproduce cleaning steps: open `data_cleaning_log.xlsx` and re-run Excel transformation steps (or re-implement in SQL/Python if desired).

---

## Contact / where this sits in my portfolio
This project demonstrates the full analyst workflow: **data hygiene → feature engineering → story-driven visual analytics → actionable business recommendations**. It’s a core project in my portfolio that I discuss in interviews to illustrate how I prioritize business impact and reproducibility.  
If you'd like a condensed resume bullet or script for explaining this project in a 60–90 second interview answer, I can provide that next.

---
