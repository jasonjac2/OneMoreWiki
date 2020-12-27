OneMore is an add-in for Microsoft OneNote 2019 that adds powerful yet simple and effective features.

* Integrated with the OneNote ribbon, context menus, and keyboard shortcuts for easy access
* [Customize the Text context menu](Settings) to add OneMore commands or a a custom search engine
* Apply [colorized syntax highlighting](Edit-Commands) to snippets of source code
* Create/edit/apply [custom styles](Custom-Styles) with advanced options
* Manage menu of [Favorites](Favorites) for one-click link to your most referenced pages
* Add [formulas](Formula-Commands) to table cell using Excel-like expressions

*Want more from OneMore? OneMore has more...* Click the pages on the right to discover all the gritty details ---->

![Screenshot](images/Screenshot.png)

### Minimum Prerequisites
* Developed for Windows 10
* Microsoft Visual Studio 2019, C# 7
* Microsoft Visual Studio 2019 Installer Projects extension
* .NET Framework 4.8
* Microsoft OneNote 2016 32-bit or 64-bit (should also work with OneNote 2013)

Tested recently with Windows 10 2004 (19041.450), VS2019, and OneNote 2019/O365

### How to Install
1. Close OneNote if it is currently running
2. Download the [latest installer from here](https://github.com/stevencohn/OneMore/releases/latest)
3. Right-click the downloaded installer msi and choose Properties, then tick the Unblock box and click OK
4. Run the installer
5. Run OneNote and enjoy

If you have issues, see the quick [trouble shooting guide](Troubleshooting). If that doesn't solve your issue then please [submit a new ticket](https://github.com/stevencohn/OneMore/issues/new/choose).

<a name="keys"></a>
## Key Shortcut Bindings
While all commands can be accessed from the OneMore ribbon group menus, some
commands also have their own key bindings. See also OneNote's 
[built-in keyboard shortcuts here](https://support.microsoft.com/en-us/office/keyboard-shortcuts-in-onenote-44b8b3f4-c274-4bcc-a089-e80fdcc87950)

| Category    | Command                       | Key Binding |
| ----------- | ----------------------------- | ----------- |
| [Editing](../wiki/Edit-Commands) | No Spell Check | F4
|             | Paste Rich Text               | Ctrl + Alt + V
|             | To uppercase                  | Ctrl + Shift + Alt + U
|             | To lowercase                  | Ctrl + Shift + U
|             | Increase font size            | Ctrl + Alt + Plus
|             | Decrease font size            | Ctrl + Alt + Minus
| [Footnotes](../wiki/Footnote-Commands) | Add footnote | Ctrl + Alt + F
|             | Remove footnote               | Ctrl + Shift + F
| [Formulas](../wiki/Formula-Commands) | Add/Edit formula | F5
|             | Recalculate formulas          | Shift + F5
| [Search](../wiki/Search-Commands) | Search and Replace | Ctrl + H
|             | Search and Move/Copy          | Alt + F
|             | Tag page                      | Alt + T
|             | Find tagged pages             | Ctrl + Alt + T
| [Snippets](../wiki/Snippets-Commands) | Insert Code Block | F6
|             | Insert horizontal line        | Shift + Alt + Minus
|             | Insert double horizontal line | Shift + Alt + Equals
|             | Insert Sortable Date          | Ctrl + Shift + D
| [Tools](../wiki/Tools) | Show XML                      | Ctrl + Shift + Alt + X
|             | Dump diagnostic info to log   | F8
|             | Clear the diagnostic log file | Ctrl + F8