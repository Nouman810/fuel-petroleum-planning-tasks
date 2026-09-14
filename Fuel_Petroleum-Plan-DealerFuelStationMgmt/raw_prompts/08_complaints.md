# Task 08: Complaints

**Depends on:** Task 04 (station management)

When something goes wrong at a station — equipment fault, delivery issue, anything — a dealer needs a way to flag it, and Admin needs a queue to work through rather than complaints getting lost in phone calls or chat.

Build the complaint flow:
- **Dealer:** submit a complaint tied to one of their own stations (subject + description). View the status of their own complaints.
- **Admin:** view all complaints across the network, update status (open → in progress → resolved/closed), and see which station and dealer each one belongs to.

This doesn't depend on orders, products, or equipment — it only needs a station to point at — so it can be built independently once stations exist. Reuse the dealer-scoping pattern from earlier tasks.

See full architecture plan: E:/Fuel_Petroleum/Planning_Tasks/Fuel_Petroleum-Plan-DealerFuelStationMgmt/spec.md
