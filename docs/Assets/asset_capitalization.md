# Asset Capitalization

The Asset Capitalization feature lets you do the following:

1. Convert one or more stock items into a new composite asset
2. Convert one or more stock items into a new composite asset and capitalize the service expenses’ cost
3. Convert one or more assets into a new composite asset

To access the Asset Capitalization feature, go to:

`Home > Assets > Maintenance > Asset Capitalization`

Let’s go through the aforementioned use cases one by one.

**1. Convert one or more stock items into a new composite asset** 

**Steps:**

* Create a new Asset Capitalization
* If you want a new composite Asset to be created, choose the Capitalization Method as "Create a new composite asset" and set the Target Item Code to the fixed asset Item to be linked with the new asset and the * Target Asset Location to the Location of the new asset. If you want a WIP composite asset to be used, choose the Capitalization Method as "Choose a WIP composite asset" and set the Target Asset to the composite asset.
* Change the Naming Series, Company, Finance Book and Posting Date if needed
* Enter the stock items to be converted in Consumed Stock Items. If you chose the Capitalization Method as "Choose a WIP composite asset", all the items tagged to the asset through Purchase Receipts/Invoices will be fetched automatically.
* Save and Submit
* Set the depreciation details (if any) of the newly created asset and submit it.

**Accounting effect:**

* The Consumed Stock Items will be reduced by the selected qty from the selected warehouses and the Warehouse Stock Accounts will be credited with the issued stock value amount.
* The system will first check if the target asset is in CWIP (Capital Work in Progress). If so, the CWIP account will be debited by the total value.
* Upon submission of the target asset, the CWIP account will be credited, and the corresponding Fixed Asset account will be debited.

**2. Convert one or more stock items into a new composite asset and capitalize the service expenses’ cost**

The prerequisites, steps and accounting effect for this is almost the same as the previous one, the only addition being that you can add the Service Expenses, and the Expense Accounts of the services would be credited with the service’s amount.

**3. Convert one or more assets into a new composite asset**

**Prerequisites:**

A new fixed asset Item (with Is Fixed Asset checkbox ticked) since it would be the item linked with the new asset.

**Steps:**

1. Create a new Asset Capitalization
2. Set the Target Item Code to the Item to be linked with the new asset
3. Set the Target Asset Location to the Location of the new asset
4. Change the Naming Series, Company, Finance Book and Posting Date if needed
5. Enter the assets to be converted in Consumed Assets
6. Save and Submit
7. Set the depreciation details (if any) of the newly created asset and submit it.

**Accounting effect:**

* The Consumed Assets will be depreciated (if configured for depreciation) till the posting date and Depreciation Journal Entries will be created in the background. Then they would be disposed of and their status would be set to "Capitalized".
* The system will check if the newly created asset is in CWIP. If it is, the CWIP account will be debited by the remaining amount of the asset after depreciation and the Accumulated Depreciation accounts will be debited by their total accumulated depreciation
* The Fixed Asset accounts of the Consumed Assets will be credited by their gross purchase amount.
* Upon submission of the newly created asset or target asset, the CWIP account will be credited, and the corresponding Fixed Asset account will be debited.