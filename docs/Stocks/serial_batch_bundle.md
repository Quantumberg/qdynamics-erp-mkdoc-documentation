# Serial and Batch Bundle

`NOTE: Users must create separate "Serial and Batch Bundles" for each stock transaction. They cannot use the same "Serial and Batch Bundle" across multiple stock transactions.


**How does this work?**

You need a Serial and Batch bundle to be created and linked to stock transactions whenever you have to deal with Serial / Batch numbers. The user needs to create a separate "Serial and Batch Bundle" for each transaction and they can't link the same "Serial and Batch Bundle" to multiple transactions.

**Auto Creation of Serial and Batch Bundle for Inward Entry**

If the user wants to create an auto "Serial and Batch Bundle" for the inward entry then they have to make sure that 'Serial Number Series' has been set for the item Serial Item and the 'Automatically Create New Batch' checkbox with 'Batch Number Series' has set for the Batch Item.

After the configuration when the user creates the Purchase Receipt or Stock Entry with the Type "Material Receipt", the system will create the "Serial and Batch Bundle" for inward automatically on submission of the record.

**Auto Creation of Serial and Batch Bundle for Outward Entry**

If the user wants to create an auto "Serial and Batch Bundle" for the outward entry then they have to enable the checkbox "Auto Create Serial and Batch Bundle For Outward" in the stock settings. The user can also set "Pick Serial / Batch Based On" as "FIFO / LIFO / Expiry" in the stock settings.

After the configuration when the user creates the Delivery Note or Stock Entry with the Type "Material Issue", the system will create the "Serial and Batch Bundle" for outward automatically on submission of the record.

**Manual Creation of Serial and Batch Bundle for Inward Entry**

For the "Serial and Batch Bundle", both serial / batch no needs to be present first in the system. So with the manual option user has to first create the Serial / Batch Nos in the system. The user has to use the CSV import option to make Serial / Batch Nos. The blank CSV template can be downloaded using the Serial and Batch Selector.

Complete GIF for manual creation of Serial and Batch Bundle for inward entry is as follow

**Manual Creation of Serial and Batch Bundle for Outward Entry**

Using the Serial and Batch Selector, the user can pick the Serial / Batch Nos based on the "FIFO / LIFO / Expiry" method.

Complete GIF for manual creation of Serial and Batch Bundle for outward entry is as follow

**History of Serial Numbers**

To check the history of Serial Numbers, check the report "Serial No Ledger"

**Serial / Batch Selector**

Is used to select Serial Nos / Batches manually, also this popup is used to create serial nos / batches automatically if they are not exists.

**Disable Serial / Batch Selector**

If users don't want to use the Serial and Batch Selector (popup) then they can disable it through Stock Settings. To disable it, goto Stock Settings > Serial and Batch Item (TAB) > "Disable Serial No And Batch Selector" enable this checkbox and save.

**Old Serial / Batch Fields**
    
Many customers have requested to retain the old serial and batch fields to address UX issues. In response to their demand, we have retained the old serial/batch fields. These fields are solely used for entering serial numbers and batches. The system will automatically create the Serial and Batch Bundle upon the submission of the stock transaction. To enable this feature, users must navigate to Stock Settings and enable the 'Use Serial / Batch Fields' option (see below image).

After that when user create the stock transaction like delivery note, system will show the old Serial / Batch Fields. 