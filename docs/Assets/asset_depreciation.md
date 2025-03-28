# Depreciation Calculation 

The system automatically creates a depreciation schedule based on the Depreciation Method, Total Number of Depreciations, and other related inputs like Available to Use Date in the Asset record. It is also possible to create multiple depreciation schedules for different Finance Books.

You need to tick the Calculate Depreciation checkbox while creating an asset if you want the system to create the depreciation schedule.

**Different Depreciation Methods** 

**Straight Line** 

In this method, the value of an asset is reduced uniformly over its useful life until it reaches its salvage value.

Example: If the asset is worth 1000 and its salvage value is 500 after 5 years, the straight line method would depreciate the asset by 100 every month/year. This method is useful when there is no particular pattern to how the depreciation takes place over a period of time.



You can use the Depreciate based on daily pro-rata option if you want the depreciation amount to vary depending on the number of days in a calendar period. You can also use the Depreciate based on shifts option to define the number of shifts the asset would run in a period in order to depreciate it accordingly. You need to first define the shift names with their shift factors in the Asset Shift Factor doctype (for example: "half": 0.5, "single": 1, "double": 1.5, and "triple": 2) and set a default. Later, if you want to change the shifts of an asset for a particular period, you can do so using the Asset Shift Allocation doctype, and the remaining shifts are automatically adjusted.

**Double Declining Balance**

This is also known as the 200% declining balance. This method is useful when the asset depreciates fast in the beginning and slows down later.

Example: If the asset is worth 100,000 and its salvage value is 11,000 after 8 years, the depreciation schedule would be:



**Written Down Value**

In this method, you can set a particular rate of depreciation or let the system calculate the rate of depreciation based on the asset’s purchase amount, salvage value, and useful life. The rate of depreciation is applied to the current written down value of the asset to calculate the depreciation amount for each year. This method is useful for assets that have higher depreciation in the initial years.

Example: If the asset’s purchase amount is 1,000 and the rate of depreciation is 40% over 5 years, the depreciation schedule would be:



**Manual**

In this method, a system-generated depreciation schedule is created for your convenience based on the depreciation details set. You can then edit the schedule dates and depreciation amounts manually for any period according to your needs.

**Automatic Depreciation Entries**

You can enable automatic booking of depreciation entries from Accounts Settings. This will create depreciation entries automatically on the scheduled dates. Otherwise, you have to create the Journal Entry manually by clicking the Make Depreciation Entry button in the corresponding Depreciation Schedule row.

**Accounting Entries on Depreciation**

In the depreciation entry:

1. Accumulated Depreciation Account is credited.
2. Depreciation Expense Account is debited.

The related accounts can be set in the Asset Category or Company.

**Asset Value Chart**
 
For better understanding, the net value of the asset on different depreciation dates is shown in a line graph. Asset Graph