# 🛒 BlinkIT Grocery Sales Dashboard | Power BI

An interactive Power BI dashboard analyzing sales performance for BlinkIT — one of India's leading quick-commerce grocery apps — across outlets, product categories, and store formats.

![Dashboard Preview](https://raw.githubusercontent.com/palakgoyal1174-debug/BlinkIT_Dashboard/main)

---

## 📌 Project Overview

BlinkIT operates thousands of outlets across India, each stocking hundreds of grocery items. This project explores a real-world business question:

> **Where is BlinkIT's revenue actually coming from — which outlets, which store formats, and which products — and what does that mean for inventory and expansion decisions?**

The dashboard turns a flat, 8,500+ row item-level dataset into a single-page, decision-ready report that a category manager or operations lead could use to spot trends at a glance.

---

## 📊 Key Insights

| Insight | Detail |
|---|---|
| **Total performance** | $1.20M in total sales across 8,523 items, averaging a 3.9/5 customer rating |
| **Outlet tier gap** | Tier 3 outlets generate ~40% more sales than Tier 1 ($472K vs. $336K) — smaller markets are outperforming |
| **Format concentration** | Supermarket Type1 alone drives ~65% of outlet-type sales ($787K of $1.20M) — a clear revenue engine worth flagging |
| **Category leaders** | Fruits & Snacks top all 16 item categories at $0.18M each; Seafood and Breakfast items lag furthest behind |
| **Growth signal** | Outlet establishment trend shows a sharp sales spike around 2018, hinting at a possible expansion phase worth investigating |

---

## 🛠️ Built With

- **Power BI Desktop** — report design & data modeling
- **DAX** — custom measures (`Total Sales`, `Avg Sales`, `No. of Items`, `Average Rating`)
- **Power Query** — data shaping and cleanup

---

## ✨ Dashboard Features

- **KPI Cards** — headline metrics with custom branded icons for instant readability
- **Outlet Establishment Trend** — line chart tracking sales across outlet founding years
- **Outlet Breakdown** — donut chart (outlet size) + funnel chart (location type) + pivot table (outlet type: Total Sales, No. of Items, Avg Sales, Avg Rating, Item Visibility)
- **Product Analysis** — bar chart ranking all 16 item types by sales, donut chart by fat content, and a clustered bar chart cross-cutting fat content by outlet location
- **Interactivity** — cross-filtering slicers for Outlet Location Type, Outlet Size, and Item Type
- **Design** — custom dark/yellow branded theme matching BlinkIT's identity, consistent visual hierarchy

---

## 🧮 DAX Measures

```DAX
Total Sales = SUM('BlinkIT Grocery Data'[Sales])

Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

No. of Items = COUNTROWS('BlinkIT Grocery Data')

Average rating = AVERAGE('BlinkIT Grocery Data'[Rating])
```

---

## 🗂️ Dataset

Item-level transactional data with the following fields:

`Item Identifier` · `Item Type` · `Item Fat Content` · `Item Weight` · `Item Visibility` · `Sales` · `Rating` · `Outlet Identifier` · `Outlet Establishment Year` · `Outlet Size` · `Outlet Location Type` · `Outlet Type`

---

## 📁 Repository Structure

```
├── BlinkIT_Grocery_Data.xlsx     # Raw dataset
├── BlinkIT_Dashboard.pbix        # Power BI report file
├── screenshot.png                # Dashboard preview image
└── README.md                     # Project documentation
```

---

## 🚀 How to Use

1. Clone this repository
2. Open `BlinkIT_Dashboard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
3. Explore the report using the slicers on the right panel to filter by Outlet Location, Size, or Item Type

---

## 👤 About Me

I'm a BSC graduate student pursuing a Data Analytics course , building a portfolio of Power BI and SQL projects as I work toward a Data Analyst role. Feedback and suggestions are always welcome!

---

⭐ If you found this project useful, consider giving it a star!
