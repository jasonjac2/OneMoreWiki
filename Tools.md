## Plugins
OneMore has a plugin facility that let you process a page using a program that you write.
This provides a simple way to experiment with page adjustments; it is an experimental
feature.

> _NOTICE: I provide no guarantee, warranty, or promise that you won't screw it up and loose data! It's in your
hands and if you mess up the XML and cause data loss, that's entirely on you. You've been warned._

Given a plugin written in PowerShell then specify the Plugin Command as powershell.exe and use the Arguments
line to specify the -file argument pointing to your plugin script as shown here.

> ![Plugin Dialog](images/PluginDialog.png)

The workflow is very simple: 

1. Create a plugin program that accepts one command line argument;
   the argument will specify the path to a file containing the page XML.
1. Run the Plugin command, specifying the path to the program and any other arguments.
1. The plugin must complete within 20 seconds or it will timeout and be aborted.
1. The plugin must write any desired changes back to the file path it was given.
1. If the plugin completes and _has made changes to the XML file on disk_ then OneMore
   will update the current page with your updated XML from the file;
1. If the plugin completes and has not made changes to the file then no changes are made
   to the current page.
1. If you chose to create a new page then it will be created regardless of whether the plugin updated the XML file.

Any output that your plugin writes to stdout will be captured in the OneMore log file.

Note, if you run the plugin and a Web browser is invoked (IE) showing the XML file contents then
you probably forgot to specify the right arguments to powershell.exe or python.exe.

The OneNote page schema is defined in the 0336.OneNoteApplication_2013.xsd file in the Properties folder of the project repo.

## XML Dialog

Developing OneMore meant reverse-engineering the way Microsoft built OneNote. And it's XML
schema reference documentation was only half the picture. This editor became invaluable
while trying to decipher the behavior and how OneNote manages its page content.

> ![XML Dialog](images/XmlDialog.jpg)

