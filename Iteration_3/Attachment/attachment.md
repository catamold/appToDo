---
title: Attachment
parent: Iteration 3
has_children: false
---

## Read / Write BLOBs from / to SQL Server using C#
Data can be exported into XML files for each users in a general format, so that it can be used for other applications. This will ensure users that they will not lose their data. Also they can import other XML files from other applications to the application.

**Example of _.xml file**
```
<?xml version="1.0" encoding="utf-8"?>
<Reminders>
	<Task title="Shopping" note="Buy some candies for Andrei\'s birthday in Barcelona and be there at 15:30 \n[ ] Present \n[ ] Cookies\n[ ] Drinks" priority="DATE" date="30-May-19 15:30:00 PM" tags="#party #music #present" status="False" />
	<Task title="Book a hotel" note="Make a reservation in New-York for 2 people." priority="This Evening" date="15-May-19 12:00:00 PM" tags="#booking" status="True" />
</Reminders>
```

![Diagram](../../images/final-assignment/SQL.png)