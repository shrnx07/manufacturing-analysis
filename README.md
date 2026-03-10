# U.S. Manufacturing Health Dashboard (1992–2025)

## Business Question
Which indicators best predict operational stress in U.S. manufacturing, 
and how quickly do disruptions propagate through orders, shipments, and inventories?

## Key Findings
- **Orders lead PPI by 2 months** (r=0.58, p<0.0001) — demand shifts before 
  input costs follow, meaning procurement teams watching PPI are systematically 
  behind the signal
- **2008 crisis was nearly twice as severe as COVID** — Durable goods orders 
  fell 37.7% YoY in March 2009 vs 19.3% in April 2020
- **70 consecutive months below average orders-to-inventory ratio (2020–2025)** 
  — suggests a structural inventory overhang, not a cyclical dip

## Live Dashboard
[View on Tableau Public](https://public.tableau.com/views/USManufacturingHealthDashboard1992-2025)

## Project Structure
```
manufacturing-analysis/
  /data        — Raw FRED datasets + cleaned combined CSV
  /notebooks   — Jupyter notebooks + exported charts
  /sql         — Analytical SQL queries (SQLite)
  /report      — One-page business brief (PDF)
```

## Data Sources
- [FRED — Durable Goods Orders (DGORDER)](https://fred.stlouisfed.org/series/DGORDER)
- [FRED — Total Mfg New Orders (AMTMNO)](https://fred.stlouisfed.org/series/AMTMNO)
- [FRED — Total Mfg Shipments (AMTMVS)](https://fred.stlouisfed.org/series/AMTMVS)
- [FRED — Total Mfg Inventories (AMTMTI)](https://fred.stlouisfed.org/series/AMTMTI)
- [FRED — Producer Price Index (PPIACO)](https://fred.stlouisfed.org/series/PPIACO)

## Tools
Python | Pandas | SciPy | Matplotlib | SQL | Tableau Public

## Key Skills Demonstrated
- Time series analysis and trend decomposition
- Lag correlation analysis between economic indicators
- Inventory stress metric design
- Business-focused data storytelling for non-technical stakeholders
