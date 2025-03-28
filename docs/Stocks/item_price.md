# Item Price 

**Item Price is the record in which you can log the selling and buying rate of an item.**

**1. How to create Item Price** 

There are two ways to reach a new Item Price form:

* Selling/Buying/Stock > Items and Pricing > Item Price > New.

Or

* Stock > Item > Click on "+" next to Item Price.

1. Select the Item. The name, UoM and description will be fetched.
2. Select the Price List whether Selling/Buying price or any other price list you may have created.
3. Enter the actual rate in the Rate field.
4. Save.

**1.1 Selecting the Price List**

You can create multiple Price Lists for one Item to track Selling and Buying Price of an Item separately. Also if the Item's selling prices change based on Territory or due to other criteria, you can create multiple Selling Price Lists for it.

On selection of Price List, its currency and applicability whether for selling/buying or both will be fetched as well. To have Item Price fetching in the sales or purchase transaction, you should have 'Price List' selected in the transaction under Currency and Price List.

To check all Item Prices together, go to:

`Stock > Stock Reports > Item Price Stock`

**2. Features**

**2.1 Unit of Measurement (UOM)**

User can add UOM specific item prices if one item is sold in differnt UOMs. For Eg: Lets say an item Rice is sold in 1 KG and 500 grams packet then users can mention the UOM in the item prices and based on the UOM selected in the transaction Item Prcie will be applied

**2.2 Packing Unit**

This is the quantity that must be bought or sold per unit of measure. For example, if Packing Unit is two, and UOM is one, two items in quantity will be transacted. The default is 0, you can use non-integer UoM like 1.5Kg Oats for 1 Packing Unit. If you leave it as 0, it'll not affect any transaction.

**2.3 Minimum quantity**

This is the minimum quantity of items to be transacted for this price to be applicable and updated in the Item Price list.

**2.4 Applying Price List to a specific Customer/Supplier**

If you select a Selling Price list, a customer field will appear where you can assign this Item Price to a specific customer. Likewise, if you select a Buying Price List, a Supplier field will appear where you can select a specific Supplier

**2.5 Applying Price List to a specific Batch**

You can also link a specific batch to an Item Price and on the selection of that batch in the transaction, the item price for that specific batch will be applied.

**2.6 Validity** 

There are two fields here—'Valid From' and 'Valid Upto'. Valid from is set to the date you created the Item Price, you can also set the Valid Upto date on which the Item Price will expire.

**2.7 Lead Time in days**

The approximate number of days it takes the product to reach the warehouse. You can set different Item Prices based on how much time the same product will reach you from different vendors.

**2.8 Note**
 
You can add any note about the Item Price in this field.