# Task 09: Sales & Shift-Closing Entry

**Depends on:** Task 05 (equipment management)

This is the daily operational heartbeat of the whole system. At the end of every shift, a dealer needs to record how much fuel each nozzle sold, and that number needs to be trustworthy since it's the basis for revenue and, later, Admin's sales reporting.

Build the shift-closing entry flow for Dealers: for a given station, shift (morning/evening/night), and date, record an opening and closing meter reading per nozzle. Compute liters sold (closing minus opening) and total amount (liters × the product's current price) automatically — don't make the dealer calculate it.

The critical business rule: a shift's opening reading for a nozzle must match that same nozzle's closing reading from its previous shift. Investigate how the nozzle's `currentMeterReading` is tracked (Task 05) so you can both validate against it and update it when a new entry is saved — this needs to happen atomically, since a sales entry and a meter-reading update are really one operation. Reject the entry with a clear error if the readings don't line up or if closing is less than opening.

Give the Dealer a simple history view of their past shift entries per station. No Admin UI in this task — Admin will consume this data through reporting in Task 10.

See full architecture plan: E:/Fuel_Petroleum/Planning_Tasks/Fuel_Petroleum-Plan-DealerFuelStationMgmt/spec.md
