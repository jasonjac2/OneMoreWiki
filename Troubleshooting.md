Software doesn't have defects. Programmers do. And I'm no exception. So what should you do if OneMore doesn't seen to be doing what it should be doing?

1. Check the log file! This is your first stop for diagnosing problems. OneMore writes a lot file to %TEMP%\OneMore.log. You can easily get to this from the hyperlink on the OneMore About dialog, presuming OneMore is working enough so you can get there. But often, errors will be written to this log file. When submitting a bug, copy any exceptions in this log file to the issue ticket.

1. Try hiding or removing the settings. OneMore stores its settings in the %APPDATA%\OneMore folder. You can rename this folder to hide it temporarily. Any new settings stored by OneMore will recreate the folder. If you discover this is not the problem, you can restore your renamed folder. But if there is a problem here, submit a new bug and attach your Settings.xml file.

1. If OneMore doesn't load at all, the best thing to try is to uninstall it and then reinstall. If you don't already have the latest version, download it and give it a try. I try to keep up with defect tickets and address them as quickly as possible.

1. You can check that OneMore is registered correctly in the Windows System Registry. If you dare, you can poke around by following the settings listed on the [Developer Notes](Developer-Notes) page in this wiki. 

As always, if you need to submit a bug, please collect as much information as you can so that I can try to reproduce the problem. 

Thank you for your patience and support.