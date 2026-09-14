# Task 10: Reporting & Dashboards

**Depends on:** Task 03 (dealer management), Task 04 (station management), Task 06 (product catalog), Task 07 (order management), Task 09 (sales & shift-closing entry)

This is the payoff task — everything Admin has been managing (dealers, stations, products, orders) and everything dealers have been recording (shift sales) needs to come together into dashboards Admin actually uses to run the business.

Build Admin-only reporting views, sliced these ways:
- Dealer-wise: total sales per dealer, across all their stations
- Station-wise: total sales per individual station
- Product-wise: sales broken down by product (MS, HSD, each lubricant SKU)
- Region-wise: sales aggregated by region
- Lubricant-wise: a dedicated breakdown of lubricant sales specifically, since it's called out separately from fuel

Investigate the shift-sales-entry data from Task 09 and the order data from Task 07 — reporting should be built as aggregation queries over that existing data, not a separate analytics pipeline or duplicated data store. Support a date range filter (e.g. this week, this month, custom range) since "sales so far" isn't as useful as "sales this month."

Keep the initial version to numbers and simple tables/charts — don't over-invest in visualization polish before confirming the underlying aggregations are correct.

See full architecture plan: E:/Fuel_Petroleum/Planning_Tasks/Fuel_Petroleum-Plan-DealerFuelStationMgmt/spec.md
