Software doesn't have defects. Programmers do. And I'm no exception. So what should you do if OneMore doesn't seen to be doing what it should be doing?

1. Check the log file! This is your first stop for diagnosing problems. OneMore writes a lot file to %TEMP%\OneMore.log. You can easily get to this from the hyperlink on the OneMore About dialog, presuming OneMore is working enough so you can get there. But often, errors will be written to this log file. When submitting a bug, copy any exceptions in this log file to the issue ticket.

1. Try hiding or removing the settings. OneMore stores its settings in the %APPDATA%\OneMore folder. You can rename this folder to hide it temporarily. Any new settings stored by OneMore will recreate the folder. If you discover this is not the problem, you can restore your renamed folder. But if there is a problem here, submit a new bug and attach your Settings.xml file.

1. OneMore runs as a separate process called dllhost.exe. This is the generic name for Windows services so you'll find many of them. To identify the OneMore process, add the "Command line" column in the Details tab of Task Manager and look for the dllhost that runs out of C:\Windows\SysWOW64 and has a parameter that starts /Processid:{88AB... If this process doesn't show up after starting OneNote then you know that the add-in is not loading.

1. If OneMore doesn't load at all, the best thing to try is to uninstall it and then reinstall. If you don't already have the latest version, download it and give it a try. I try to keep up with defect tickets and address them as quickly as possible.

1. Check that OneMore is registered correctly in the Windows System Registry. If you dare, you can poke around by following the settings listed on the [Developer Notes](~-Developer-Notes) page in this wiki. 

1. If OneNote is installed for _all users_ then OneMore must also be installed for _all users_.

1. If you're running on a 64-bit machine then either the 64-bit or 32-bit installer will work. But if you're running on a 32-bit machine then you must use the 32-bit installer. This is an installer issue; OneMore is built identically for both.

1. If you see an error dialog that says something like "OneMore failed to connect to OneNote" then it's likely due to a bad OneNote configuration. Try to run the Office installer and choosing the Repair option. This will repair Office and OneNote and may clear up the connection issue.

As always, if you need to submit a bug, please collect as much information as you can so that I can try to reproduce the problem. 

Thank you for your patience and support.

# OneNote Specific Problems

## Search is Flaky
Some OneMore commands, such as the _Link References_ command, use the internal search capabilities of OneNote. This is based on the Windows Search engine which indexes content on your computer. Sometimes it takes a while for the index to synchronize with recent changes in your notebooks. Sometimes it doesn't synchronize at all which means you don't find what you're looking for, or commands like _Link References_ don't seem to work.

To correct this, there are two possibilities. First, you can try rebuilding the Windows Search index for OneNote.

1. Open the Windows Start menu and type _Indexing Options_ and press Enter
1. Select _Microsoft OneNote_ and click the _Advanced_ button
1. Click the _Rebuild_ button next to "Delete and rebuild index"
1. Press OK. This may take some time (hours maybe)

Second, if that doesn't seem to work, you can delete the OneNote cache

1. Close OneNote
1. Open Windows File Explorer
1. Navigate to the cache folder, something like C:\Users\_username_\AppData\Local\Microsoft\OneNote\16.0\cache
1. Delete everything in this folder
1. Open OneNote. It will reload all of your notebooks, sections, and pages. This will appear slow because it's rebuilding that cache folder.
