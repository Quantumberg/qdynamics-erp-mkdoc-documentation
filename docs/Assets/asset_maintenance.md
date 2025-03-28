# Asset Maintenance 

**Asset Maintenance refers to any activity done on Assets to maintain their performance or condition.**

It provides features to track the details of individual maintenance/calibration tasks for an asset by date, the person responsible for the maintenance, and future maintenance due date.

To perform Asset Maintenance:

1. Enable 'Maintenance Required' from the Asset master.
2. Create an Asset Maintenance Team.
3. Create the Asset Maintenance.
4. An Asset Maintenance Log is created.
5. Create Asset Repair Log.

To access the Asset Maintenance list, go to: > Home > Assets > Maintenance > Asset Maintenance

**1. Prerequisites**

Before creating and using Asset Maintenance, it is advised to create the following first:

* Asset with 'Maintenance Required' checked.
* Asset Maintenance Team

**2. How to create Asset Maintenance**

For each asset, create an Asset Maintenance record listing all the associated maintenance tasks, maintenance type (Preventive Maintenance or Calibration), periodicity, assign to and start and end date of maintenance. Based on start date and periodicity the next due date is auto-calculated and a ToDo is created for the Assignee.

1. Go to the Asset Maintenance list, click on New.
2. Select the Asset.
3. Select the Asset Maintenance Team.
4. Add Maintenance Tasks in the table.

  1. Set the Maintenance Status whether 'Planned', 'Overdue', or 'Canceled'.
  2. Select a periodicity for which the task needs to be carried out. The next due date will be calculated.
5. Save.
6. After saving, you can assign the task to a user.

If the Item is serialized, the Serial Number can be entered.

**3. Features**

**3.1 Maintenance Tasks**

* **Maintenance Type:** Whether this is a 'Preventive' maintenance activity or 'Calibration' to restore accurate functioning.
* **Start and End Date:** Set the start date and end date when the maintenance is supposed to begin and end.
* **Last Completion Date:** If the maintenance was not carried out on or before the scheduled date, the actual date of maintenance can be recorded here.

**3.2 Asset Maintenance in ToDo** 
On assigning the maintenance to a user, it will appear in the User's ToDo list.
