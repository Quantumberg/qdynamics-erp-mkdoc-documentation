# Stock Level Report 

**Stock Level report list stock item's quantity available in a particular warehouse.**

There are multiple reports available you can check for item's stock level.

**Stock Projected Quantity Report**

This report list item wise - warehouse wise stock level of an item considering all the stock transactions. With Actual Quantity of an item, it also provide other details like:

1. Actual Qty: Quantity available in the warehouse.
2. Planned Qty: Quantity, for which, Work Order has been raised, but is pending to be manufactured.
3. Requested Qty: Quantity requested for purchase, but not ordered.
4. Ordered Qty: Quantity ordered for purchase, but not received.
5. Reserved Qty: Quantity ordered for sale, but not delivered.
6. Project Qty: Project Quantity is calculated as

Projected Qty = Actual Qty + Planned Qty + Requested Qty + Ordered Qty - Reserved Qty