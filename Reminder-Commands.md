Outlook users have the luxury of creating _tasks_ that remind them of things they need to do. Outlook and OneNote are integrated so you can create an Outlook task on a OneNote paragraph and Outlook will keep you informed of its status. But if you're a OneNote user and don't also use Outlook or don't want to pollute your Outlook tasks with OneNote-related tasks then OneMore adds a stand-alone task reminder management system to OneNote.

_Note that OneMore reminders emulate Outlook tasks but are not the same and not integrated with Outlook. OneMore reminders are intended for those who do not have Outlook. However, if you do have Outlook, you can import tasks from Outlook and also create OneMore reminders. Don't confuse them!_

## Notifications
OneMore integrates reminders with the Windows _toast_ popup notifications. These are popup notifications in the lower-right corner of the window off of the taskbar and show up in the Windows _notification area_. Clicking on one of these OneMore reminder notifications will navigate to the page containing the reminder, select the associated paragraph, and open the reminder dialog. You can then modify the reminder, or _snooze_ it for a period of time.

Note that notifications are only sent while OneNote is running. You will _not_ receive OneMore reminder notifications while OneNote is not running.

## Commands
The Reminders menu has multiple commands to create, complete, delete, and even generated detailed reports on reminders that you create in OneNote. This menu item along with all of its commands, or individual commands, can be added to the page context menu for quick access.

### Create or Update Reminder (F8)
Creates or updates a reminder for the current paragraph. The cursor must be positioned on the paragraph of interest with no text range selected. You can select one tag to associate with the reminder; it is recommended that you select a _checkable_ tag, but any tag will do.

### Complete Reminder
Marks the reminder associated with the current paragraph as complete. If the associated tag is a checkbox, it will be ticked.

### Delete Reminder
Deletes the reminder associated with the current paragraph and optionally removes the tag.

### Reminders Summary Report
Generates a detailed report page of all active and inactive reminders.

### Import Tasks from Outlook
Imports Outlook tasks in a list or tabular form. When imported as a table, the start, due, completed, and other properties are displayed. _Note that OneMore can only keep track of the status (clickable status flags) of tasks in the main Outlook Tasks folder. While OneMore can import tasks from other folders, OneNote does not keep track of their status._ 

The task detail table is accompanied by a title with a _refresh_ link. Click this link to update the task details from Outlook.

## Notes

* Reminders are linked to OneNote paragraphs. Internally, OneNote assigns an ID to each paragraph. Unfortunately, those IDs are ephemeral, generated on each machine on which you view the page at the time the page is viewed. This means that the ID for a particular paragraph changes based on the machine used to view it. This also means that a reminder created on one machine can't be managed or notified on a another machine that shares the same notebook. This is a limitation in the way OneNote works. OneMore could work around this but the solution would be highly inefficient and affect performance of OneNote and possibly your computer.

* OneMore will scan alls reminders and send notification immediately after OneNote is started. It will then continue to scan once every five minutes. You may start to see notification for a particular reminder every five minutes however this will become once every 10 minutes, then once every hour, and then once every 12 hours based on how long you have OneNote running. This simple progressive schedule is to avoid being overwhelmed when continuing to dismiss a reminder.
