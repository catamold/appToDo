---
title: Use-cases
parent: Iteration 1
has_children: true
nav_order: 1
---

## Use-cases
Next I'll present the use-cases for the application as described in Alistair Cockburn's book: _Writing Effective Use Cases_.

**Use Case Reminder**

*Primary Actor:* User

*System:* Reminder's Data
1. User adds reminders into system, by completing the following fields:
  - Title
  - Priority
  - Date
  - Note
  - Tags
  - Status

2. User choose to preview the reminder.

3. User choose to edit the reminder, changing some of the fields:
  - Title
  - Priority
  - Date
  - Note
  - Tags
  - Status
  
4. User choose to delete the reminder.

*Extensions:*

1a. Submitted data is incomplete:
  - Submission complete with no errors

3a. Submitted data is incomplete:
  - Retry Login by changing email or password

**Use Case Personal Data**

*Primary Actor:* User

*System:* ToDo Main Page
1. User can choose how reminders could be organized:
  - Inbox
  - Today
  - Upcoming
  - Anytime
  - Someday
  - Logbook

2.	User can search for reminders using a serach bar, the keywords typed in the box text will display all reminders based on their title name or hashtags used.

*Extensions:*

2a. Submitted data contains illegal characters:
  - No reminder found

**Use Case Account**

*Primary Actor:* User

*System:* Premium plan
1.	User can choose to pay in order to have benefits:
  - No ads (Main Page)
  - Customized tags (Reminder Page)
  - Unlock _This Evening_ priority (Reminder Page)
  - Notifications

**Use Case Alert System**

*Primary Actor:* Application

*System:* ToDo Main Page
1.	Based on the priority, some reminders will appear as a notification in time.