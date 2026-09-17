## 📌 Overview
This repository contains a Power BI report (`power_bi_task3.pbix`) built around Shopify stock data. The data model is loaded and ready — the report canvas itself is currently **blank / work-in-progress**, so this repo also doubles as a base to build the dashboard out from.

## 📂 Repository Contents
```
power_bi_task3.pbix     # Power BI report file
README.md               # This file
```

## 🗃️ Data Model

| Table | Description |
|---|---|
| `Shopify Stock` | Core table containing stock trading data (prices/volume). Exact columns are only viewable inside Power BI Desktop, since the model is stored in a compressed binary format. |
| `Dim_Date` | Date dimension table intended for time-based analysis (trends, YoY/MoM comparisons, filtering). |

> ⚠️ No relationship is currently defined between `Shopify Stock` and `Dim_Date`. This needs to be created (recommended: one-to-many, `Dim_Date` → `Shopify Stock`) before building time-based visuals.

## 📊 Report Details

| Property | Value |
|---|---|
| Pages | 1 (`Page 1`) |
| Canvas size | 1920 × 1080 (16:9) |
| Display mode | Fit to Page |
| Theme | Fluent 2 (Preview) |
| Visuals | None yet — blank canvas |

## 🚀 Getting Started
1. Clone this repo / download `power_bi_task3.pbix`.
2. Open it in **Power BI Desktop**.
3. Go to **Model view** and create the relationship between `Dim_Date` and `Shopify Stock`.
4. Start adding visuals (see suggestions below).

## ✅ Suggested Visuals / Next Steps
- 📈 Line chart — stock price (Open/Close/High/Low) over time
- 🧮 KPI cards — latest price, % change, volume
- 📊 Bar chart — trading volume by date
- 🎚️ Slicer — filter by date range (year/month)
- ➕ DAX measures — daily % change, moving average, YTD performance
