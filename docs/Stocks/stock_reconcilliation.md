# Stock Reconciliation

Stock Reconciliation is the process of counting and evaluating material/products, periodically at the year end.

This is done in order to:

* Keep the actual physical stock count and book stock count in sync
* Value the stock for preparation of the accounting statements

The Stock Reconciliation feature is used for:

* Posting opening stock
* Reconciling book and actual stock

To access the Stock Reconciliation list, go to: > Home > Stock > Tools > Stock Reconciliation

**1. How to Create a Stock Reconciliation to Post Opening Stock**

Using stock reconciliation you can update the number of specific items in a warehouse as of specific time. You can also add Items in the stock which have Serial Numbers or the Batch Numbers.

1. Go to the Stock Reconciliation list, click on New.
2. Select the Purpose as 'Opening Stock'. You can edit the posting Date and Time.
3. Select Item Code, Warehouse, Quantity, and Valuation Rate. If there is a Serial / Batch No involved, add it.
4. If you want to auto-generate Serial No / Batch No then keep those fields blank.

  * For auto-generation of Serial No, you need to set "Serial Number Series" in the Item master.
  * For auto-generation of Batch no, you need to enable "Automatically Create New Batch" checkbox in the item master.
5. The Difference Account will be set as 'Temporary Opening'.
6. Save and Submit.

`Note: Maintain Stock option should be enabled in Item master for this to work.`

**2. How to Create a Stock Reconciliation to Reconcile Book and Physical Stock Count**

Stock Reconciliation is the process of counting and evaluating stock-in-trade, periodically and at year-end in order to value the total stock for preparing accounting statements. In this process, the actual physical stocks are checked and recorded in the system. The actual stocks and the stock in the system should be in agreement and accurate. If they are not, you can use the Stock Reconciliation tool to reconcile stock balance and value with actuals.

To reconcile the stock:

1. Go to the Stock Reconciliation list, click on New
2. Select the Purpose as 'Stock Reconciliation'. You can edit the posting Date and Time.
3. Set Item Code, Warehouse.
4. The current Quantity and Valuation Rate will be fetched, change the quantity as required.
5. The expense account in Difference Account will be set to 'Stock Adjustment' by default.
6. The Cost Center default will be 'Main', change if needed.
7. Save and Submit.

**3. Features** 
**3.1 Upload Data Through Spreadsheet** 
If you have a lot of items, you can upload the details via a spreadsheet.

1. Download Template
Open new Stock Reconciliation and click on Download button to download the template in CSV format.

2. Enter Data in CSV Template.

The CSV format is case-sensitive. Do not edit the headers which are pre-set in the template. In the Item Code and Warehouse column, enter exact Item Code and Warehouse as created in your account. For quantity, enter the stock level you wish to set for that item, in a specific warehouse.

3. Upload the CSV file with the data by clicking on 'Upload' button.

4. Review, Save and Submit.

5. Check Stock Ledger Report for updated stock balance.

**3.2 Get Stock Balance and Valuation as of Specific Date and Time**

You can import the stock balance and valuation as of specific date and time from a selected Warehouse by clicking on Items button. You can update the Quantity and Valuation Rate as needed.

**3.3 Using barcode scanner to scan physical inventory**

If you have configured barcodes for your items you can use a barcode scanner to reconcile physical quantities. To do this follow these steps:

  1. Set default warehouse
  2. Enable "Scan Mode" this will disable fetching existing quantity and let you add quantities by incrementally scanning items.
  3. Click on "Scan Barcode" field and use your barcode scanner to send input. Reconciliation items table will will keep getting updated as you scan items. Following video demonstrates this process.

**4. How Stock Reconciliation Works** 
Once a stock reconciliation is posted to update the quantity on specific date and time for an item in a warehouse, it will not be modified by subsequent stock transactions even if such transactions have a posting date which is prior to the stock reconciliation date. In other words, backdated entries will not change the stock numbers after a Stock Reconciliation entry is posted.

Examples are as follows.

**4.1 For non-serialized Items**

Consider an item with code 'ABC001' in a 'Mumbai' warehouse. Let's assume that stock as on 10th January is 100 units. Stock Reconciliation is made on 12th January to set stock balance to 150 units.

Stock Ledger would look as shown below:

| Posting Date | Qty | Balance Qty | Voucher Type | | 10/01/2014 | 100 | 100  | Purchase Receipt | | 12/01/2014 | 150 | 150 | Stock Reconciliation |

If a new Purchase Receipt entry is made on 5th January 2014, which is prior to the date of Stock Reconciliation entry, Stock Ledger would look as shown below.

```<table border="1" cellspacing="0px">```


Posting Date Qty Balance Qty Voucher Type 05/01/2014 20 20 Purchase Receipt 10/01/2014 100 120 Purchase Receipt 12/01/2014
150 Stock Reconciliation

As you can see, the Balance Qty as on 10th January got updated from 100 to 120. But the Balance Qty as on 12th January did not get updated from 150 to 170. ### 4.2 For Serialized Items For an Item, ITEM-00225 that has has the 6 serial nos HJF00020, HJF00021, HJF00022, HJF00023, HJF00024, HJF00025 with valuation rate as 530 per serial no. At the end of the year, the user has come to know that they have only 3 Serial Nos against that item with Valuation Rate 620. So to remove the old serial nos HJF00020, HJF00021, HJF00022, HJF00023, HJF00024, HJF00025 and add the new serial nos with new Valuation Rate, Stock Reconciliation can be used as follows: Select the item ITEM-00225 in the stock reconciliation, on the selection of the Item the system will auto pull the existing serials nos. Then set Qty as 3, Valuation Rate as 530 and serial no as HJF00026, HJF00027, HJF00028.


Before reconciliation, the valuation rate was 530 and the available qty was 6, so the total stock value was 3,180. After reconciliation, the valuation rate has changed to 620 and available qty changed to 3, so the new stock value becomes 1,860. To adjust the stock value in the accounting, the system has credited extra amount 3,180 - 1,860 = 1,320 to Warehouse's account and debited to stock adjustment account. The GL entries for the above entry is as follows: To view GL entries, click on button View > Accounting Ledger 

The stock balance after submission of the stock reconciliation:

The general ledger for the warehouse account Nagpur after submission of the stock reconciliation:

### 4.3 For Batch Items Stock reconciliation for batch items will be used to add a new batch or to update the quantity of the existing batch. For example, the batch JHGJH00003 has the current quantity as 60 but if the user wants to make it 100 then by using stock reconciliation, user can update the batch quantity.

Batch-Wise Balance History report after submission of the stock reconciliation:

**5. Serial and Batch Bundle**

In version 15 the serial and batch bundle feature has introduced to make stock transaction against the serial no / batch items. For stock reconciliation, user gets two option to make serial and batch bundle.

* **Use Serial / Batch Fields:**

The user can use the old serial / batch fields to make serial and batch bundle automatically. In this case user has to enable the checkbox "
Use Serial No / Batch Fields" in the line item

* **Use Serial / Batch Bundle:**

The user can use the Serial / Batch bundle to make stock reconciliation for serialized / batched items. Here user gets option to either "Reconcile All Serial Nos / Batches" or "Reconcile Selected Serial Nos / Batches"

```+ **Reconcile Selected Serial Nos / Batches:** The user needs to disable the "**Reconcile All Serial Nos / Batches**" checkbox and create a serial and batch bundle for specific serial numbers or batches. By doing this, the system will automatically create the Current Serial / Batch Bundle for the serial numbers or batches which has been selected by the user manually within the Serial and Batch Bundle.


For example, if the user has 10 batches and wants to change the valuation rate of only 2 batches, then the user should disable the "Reconcile All Serial Nos / Batches" checkbox, and create the serial and batch bundle for those 2 batches with the new valuation rate.
+ **Reconcile All Serial Nos / Batches:** The user needs to enable the checkbox "**Reconcile All Serial Nos / Batches**" and create a serial and batch bundle.


For example, if the user has 10 batches and wants to reconcile and keep only one batch. Using the stock reconciliation, the user will be able to consume 9 batches automatically and retain one batch. For that, the user has to enable the "Reconcile All Serial Nos / Batches" checkbox in the Stock Reconciliation Item, and then the system will automatically consume 9 batches and add one batch on submission of the stock reconciliation.```