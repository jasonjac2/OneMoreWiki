## Colorize
Applies colorized syntax highlighting to selected source code. Supported languages include: 

- C#
- C++
- CSS
- Go
- HTML
- Java
- JavaScript/JSON
- PowerShell
- Python
- Typescript
- VB
- Wolfram
- XML
- YAML

For best results, first select the text you want to colorize, set the style to Code, and then colorize the selection.

The highlighting is not as complete as you might find in VS or VSCode but then OneNote isn't intended to be a programming editor anyway. However, languages are defined in JSON definition files located below the OneMore installation directory so they can be customized and enhanced and new languages can be added.

If you're so inclined to add enhancements or define a new language, please submit a pull request.

## Proofing Language
This menu is only visible if you've configured Office with two or more proofing languages. This can be done in any Office application including OneNote by going to the Options dialog and then the Languages sheet.

Sets the proofing language of selected text or the entire page to the chosen language. This can be added to the context menu.

## Increase Font Size (Ctrl + Alt + Plus)
Increases the font size of all text on the entire page. To increase the font size of selected text, use the built-in OneNote shortcut Ctrl+Shift+>

## Decrease Font Size (Ctrl + Alt + Minus)
Decreases the font size of all text on the entire page. To decrease the font size of selected text, use the built-in OneNote shortcut Ctrl+Shift+<

## To UPPERCASE (Ctrl + Shift + Alt + U)
Converts the selected text to uppercase.

## To lowercase (Ctrl + Shift + U)
Converts the selected text to lowercase.

** To Title Case
Converts the selected text to title case.

## Enable Spell Check
Enables spell checking on the current page or for the selected text by
resetting the proofing language of the page to your default culture, e.g. "en-US"

## Disable Spell Check (F4)
Disables spell checking on the current page or for the selected text by
setting the proofing language of the page to "yo".

## Invert Selection
Inverts the selection on the current page, de-selecting all selected content and selecting all non-selected content.

## Join Paragraph
Joins multiple selected consecutive lines into a single paragraph, eliminating soft-breaks.

## Paste as Plain Texxt (Ctrl + Shift + V)
Pastes the contents of the clipboard as plain text.

## Paste Rich Text (Ctrl + Alt + V)
Pastes rich text from the clipboard, preserving formatting and colors.

## Rotating Highlighter (Ctrl + Shift + H)
Uses a rotating array of colors to highlight selected text. Each time you select text and use this command, it will highlight the selected text using the next color in the array. Choose the color theme from the Settings dialog.
> ![Rotating Highlighter](images/Rotating.png)

## Select All Images
Select all images on the page. This can be used, for example, to delete all images quickly and easily.

## Select Text with Similar Formatting
Selects all content with the same style treatment as the selected text. The selected text is either inferred from the insertion cursor or an explicitly selected region. Once selected, one or sometimes more commands can be executed to affect the selected text ranges. For example, you could select all Heading 2 headings and change the color and make them italic.

Note that OneNote does not allow multiple non-contiguous selection ranges within a single paragraph. This may result in selecting only the last range in the paragraph that meets the style criteria. This is the way that OneNote works so a little extra manual work may be needed to make additional edits.

> ![Selet Similar Formatting](images/SelectStyle.gif)

## Sort Lists
Sorts the current list or all lists on the page, with options to sort nested lists and numeric lists.

