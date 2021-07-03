Adding footnotes to a OneNote page seems somehow redundant but consider how often OneNote
is used for research and then used to copy/paste content into Word or print as PDF... yeah,
you get it then.

## Add Footnote (Ctrl + Alt + F)
You can add a footnote anywhere on the page and a reference label is inserted at the current
cursor location and a footnote is added to the bottom of the page. You can then edit the
text in that footnote to your heart's desire. Text colors are based on the page background color.

> ![Footnotes](images/Footnotes.png)

Note that footnotes are hyperlinked so you jump from the content body down to the text
of a footnote or back up again to the content that references a particular footnote.

## Insert QR Code
Converts selected text to a QR code and inserts the QR image into a new paragraph following the selected text. QR codes provide a convenient way to share passwords, Web addresses, any other data (up to 2000 characters).

## Link References To This Page
Creates bi-directional reference links between the current page and pages that reference this page by its title. All instances of the page title on referring pages are converted to hyperlinks back to this page and a _Linked References_ sections is appended to this page with links back to all referring pages.

## Map Linked Pages
Generates a report showing all pages that contain links to other pages. This can be
scope to the current section, current notebook, or all notebooks. The report is produced
as a new page in the current section.

By default, links are scanned within the chosen scope, e.g. just the current section.
If you want to include links beyond the current scope, check the _Include cross-notebook
references_ checkbox. Depending on the number of pages and notebooks, this can be time consuming.

## Refresh Footnotes
Refreshes all footnote references on the page so their numbers are sequential on the page. 
This is useful when moving content up or down the page.

## Remove Footnote (Ctrl + Shift + F)
And if you no longer want a footnote, place the cursor over the label or over the footnote
text at the bottom of the page and click the *Remove footnote* command. Voila!

OneMore keeps track of footnotes and will automatically reorder them to keep them numbered
sequentially from the top of the page. If you delete a footnote, it again will renumber
the remaining footnotes so there are no gaps. Pretty slick, huh?

## Replace URLs with Images
Replaces all or selected hyperlinked URLs that reference online images with those referred image. If the image cannot be downloaded, no changes are made.

## Replace URLs with Web Page Titles
Automatically replaces all or selected hyperlinked URLs with the &lt;title> specified on the 
associated Web pages. This only affects URLs for which the displayed text is the same as the
link address, meaning if you've already customized the displayed text, OneMore will not alter
your changes.

For example, given this URL on a OneNote page: [https://github.com/](https://github.com/)

it would be replaced with its hyperlinked title: [GitHub](https://github.com)
