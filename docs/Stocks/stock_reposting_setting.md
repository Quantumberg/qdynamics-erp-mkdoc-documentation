# Stock Reposting Settings 

**Limit timeslot for Stock Reposting**

If you want to run the reposting in a specific time then you can enable the checkbox "Limit timeslot for Stock Reposting". With this configuration you can avoid deadlock issues which occurs during the reposting.

**Limits don't apply on** 
If you want to run the reposting full day and not on a specific time, especially when you have weekly off then you can use this configuration.

**Use Item Based Reposting** 
This option is helpful when you want to speed up reposting. The system skips reposting for duplicate items and warehouses to improve speed.

**Do reposting for each Stock Transaction** 
The system creates a reposting record for backdated entries. This means that the system only generates a reposting record if a future transaction exists for the same item and warehouse. We have seen cases where system has not created reposting entry for backdated transaction because of concurrency issues. So to solve them added this option which won't check whether the future transaction exists for the same item and warehouse to make reporting record. This is also added for an audit purpose.

**Notify Reposting Error to Role** 
If reposting fails due to any issues, the system sends emails to the system managers. If you don't want to send failure emails to the system managers, you can configure a role, and the system will then send the email to the users assigned to that respective role.