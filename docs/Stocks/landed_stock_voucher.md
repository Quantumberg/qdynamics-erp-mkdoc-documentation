# Landed Cost Voucher 

**Landed Cost is the final total cost associated with a product for it to reach the buyer’s doorstep.**

Landed costs include the original cost of the item, complete shipping costs, customs duties, taxes, insurance, currency conversion fees, etc. All of these components might not be applicable in every shipment, but relevant components must be considered as a part of the landed cost.

`What is Landed Cost?`

`To understand landed cost better, let’s take an example based on our daily lives. You need to purchase a new washing machine for your home. Before making an actual purchase, you probably do some research to know the best price. In this process, you often found a better deal from a store which is long away from your home. But you should also consider shipping cost while buying from that store. Total cost including shipping might be more than the price you get in your nearby store. In that case, you will choose to buy from your nearest store, as the landed cost of the item is cheaper in the nearest store.`

Similarly in business, identifying landed cost for an Item/product is very crucial, as it helps to decide selling cost of that item and impacts the company’s profitability. Hence all applicable landed cost charges should be included in Item’s valuation rate.

According to the Third-Party Logistics Study, only 45% of the respondents stated that they use Landed Cost extensively. The main reasons of not using Landed Cost were unavailability of necessary data (49%), lack of right tools (48%), insufficient time (31%), and not sure how to apply landed cost (27%).

To access the Landed Cost Voucher list, go to: > Home > Stock > Tools > Landed Cost Voucher

**1. Prerequisites**

Before creating and using Landed Cost Voucher, it is advised that you create the following first:

* A Purchase Receipt or Purchase Invoice with Update Stock enabled. This is your original receipt of goods.
* A Purchase Invoice for the landed costs (e.g. Freight, Insurance, etc.)

We will then use the Landed Cost Voucher to decrease the costs recorded through the second Purchase Invoice and increase the stock value.

**2. How to create a Landed Cost Voucher**

 1. Go to the Landed Cost Voucher list, click on New.
 2. Select Receipt Document Type whether Purchase Invoice or Receipt. You can select multiple documents.
 3. Select the specific Invoice or Receipt. The supplier name and Grand Total will be fetched automatically.
 4. Click on the Get Items from Purchase Receipts button to fetch the item details from the Purchase Invoice/Receipt.
 5. Select whether Distribute Charges Based On should be on quantity or Amount.
 6. Enter the Expense Account and the Amount for Additional Costs in the Taxes and Charges table. The amount will be distributed equally based on the quantity or amount as per your selection.
 7. Save and Submit.

In the document, you can select multiple Purchase Receipts/Invoices and fetch all items from those Purchase Receipts. Then you should add applicable charges in “Taxes and Charges” table. You can easily delete an item if the added charges do not apply to that item.

The added charges are proportionately distributed among all the items based their amount or quantity. If you selected based on the amount, the Item with the highest amount will be allocated the highest proportion of the charges. In case of quantity, Item with the highest quantity will be allocated most of the charges and the other Items will be allocated lesser amounts. 

**3. Related Actions**

**3.1 Adding Landed Cost in the Purchase Receipt itself** 

You can add landed cost-related charges in “Taxes and Charges” table while creating Purchase Receipt (PR). You should add those charges for “Total and Valuation” or “Valuation” in the 'Consider Tax or Charge for' field. Charges which are payable to the same Supplier from whom you are buying the items should be tagged as “Total and Valuation”. Otherwise, if applicable charges are payable to a 3rd party, it should be tagged as “Valuation”. On submission of Purchase Receipt, the system will calculate the landed cost of all items, considering those charges. This landed cost will be considered to calculate the item’s Valuation Rate (based on FIFO / Moving Average method).

But in reality, while making Purchase Receipt we might not know all the charges which are applicable for landed cost. Your transporter can send the invoice after 1 month, but there is no point in waiting for booking Purchase Receipt till then. Companies that import their products/parts, pay a huge amount as Customs Duty. And generally, they get invoices from the Customs Department after a while. In these cases, “Landed Cost Voucher” becomes handy, as it allows you to add those additional charges on a later date, and to update landed cost of purchased items.

**3.2 What happens on submission?** 
1. Valuation Rate of items is recalculated based on new landed cost.
2. If you are using “Perpetual Inventory”, the system will post general ledger entries to correct Stock-in-Hand balance. It will debit (increase) corresponding “warehouse account” and credit (decrease) Expense Account mentioned in Taxes and Charges table. If items are already delivered, the Cost-of-Goods-Sold (CoGS) value has been booked as per the old valuation rate. Hence, general ledger entries are reposted for all future outgoing entries of associated items, to correct CoGS value.