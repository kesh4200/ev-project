# EV Market Intelligence Dashboard

An interactive EV market analytics dashboard built with HTML, CSS, JavaScript, Plotly.js, Papa Parse, and SheetJS. It runs in the browser without a backend or API key.

## Features
- Nine visualizations: category distribution, category performance, manufacturer sales, customer ratings, annual sales trend, battery technology share, country distribution, range by battery type, and price vs range.
- Five KPI cards: record count, average battery capacity, average driving range, annual sales, and customer rating.
- Upload CSV, XLSX, or XLS datasets.
- Region, category, model year, and battery filters recalculate charts and KPIs.
- Responsive dark theme; large scatter plots are sampled for performance.

## Run
Open the repository in VS Code and use the Live Server extension to open `index.html`. Upload your CSV or Excel dataset using the upload control. External libraries load from CDNs, so an internet connection is needed. Uploaded data is processed locally in the browser and is not sent to a server.

## Expected columns
`manufacturer`, `model_name`, `model_year`, `manufacturing_country`, `market_region`, `category`, `battery_type`, `battery_capacity_kwh`, `range_km`, `price_usd`, `annual_sales_units`, `customer_rating`. Common aliases are supported; edit the `aliases` object in `index.html` if your dataset uses different names.

## Tableau handoff
For a Tableau-native dashboard, connect Tableau to the CSV dataset, create KPI worksheets and category/manufacturer/year/battery/country/range-price visualizations, apply shared filters, and assemble the worksheets into a dashboard. This repository contains a web dashboard, not a native Tableau `.twb`/`.twbx` workbook.

## Stakeholder scenarios
- EV Market Strategy Director: category demand, manufacturer sales, battery adoption, and ratings.
- Automotive BI Manager: competitive sales, manufacturing geography, and battery mix.
- Sustainable Mobility Research Analyst: range, battery technologies, geography, and adoption indicators.

Treat findings as descriptive rather than forecasts or evidence of causation; verify data provenance before business or policy use.