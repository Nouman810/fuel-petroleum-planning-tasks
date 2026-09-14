# Task 07: Order Management

**Depends on:** Task 04 (station management), Task 06 (product catalog)

Dealers need to restock fuel and lubricants at their stations, and Admin needs to track and fulfill those requests. This is the first place stations and products come together.

Build the order flow:
- **Dealer:** place an order against one of their own stations, picking a product from the catalog and a quantity. View their own orders and current status.
- **Admin:** view all orders across the network, and move an order through its lifecycle: pending → approved → dispatched → delivered. An order can also be rejected, but only before it's been delivered.

Enforce the status transitions server-side — investigate the order lifecycle in the spec before deciding on validation, but the short version is: no skipping stages, no editing a delivered order, no un-rejecting. Reuse the dealer-scoping pattern from earlier tasks so a Dealer can only see and place orders for their own stations.

See full architecture plan: E:/Fuel_Petroleum/Planning_Tasks/Fuel_Petroleum-Plan-DealerFuelStationMgmt/spec.md
