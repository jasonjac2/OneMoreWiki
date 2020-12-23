## Add Icon to Page Title
Chose from a selection of icons from the Segoe UI Emoji font to add to the page title;
OneNote automatically displays that icon in the page navigator as well.

> ![Title Icon Dialog](images/TItleIconsDialog.png)

## Collapse Pages
Collapses the page hierarchy to see only top-level pages.

## Convert Text to Table
Converts selected text to a table. Text must be delimited by a comma, space, or other special character so the command can detect columns.

> ![Text To Table](images/TextToTable.png)

## Insert Table Cells
Adds the ability to insert cells into a table, shifting existing content down or to the right.
This is similar to the Excel functionality with one enhancement - if you select a rectangular
region of cells then it will shift just those cells, possibly overwriting other cells. If you
select cells from one column or cells from one row then it will insert cells above or to the left
and add rows or columns as needed to make room for the new cells.

> ![Insert Table Cells](images/InsertCellsDialog.png)

_Note that if you move cells with formulas, the cell references in those formulas are not updated
automatically by this command; you'll need to adjust those manually._

## Insert Pronunciation
Inserts the "ruby text" pronunciation of selected words. This uses an online service that supports over a dozen languages.

## Map Linked Pages
Generates a report showing all pages that contain links to other pages. This can be scope to the current section, current notebook, or all notebooks. The report is produced as a new page in the current section.

By default, links are scanned within the chosen scope, e.g. just the current section. If you want to include links beyond the current scope, check the _Include cross-notebook references_ checkbox. Depending on the number of pages and notebooks, this can be time consuming.

## Merge pages
Merges two or more pages into a single page preserving formatting and position of outlines. 

Outlines are using in variety of ways, not the least of which to preserve some conceptual context with other containers on the page based on size and position, so OneMore doesn't attempt to merge containers from multiple pages but instead preserves the layout of containers from each page in a continuous stream in the newly merged page.

You can easily merge to containers by Shift+clicking one container and dragging it on top of the container with which you want the first to be merged. This is a built-in OneNote feature.

## Replace URLs with Web Page Titles
Automatically replaces all or selected hyperlinked URLs with the &lt;title> specified on the 
associated Web pages. This only affects URLs for which the displayed text is the same as the
link address, meaning if you've already customized the displayed text, OneMore will not alter
your changes.

For example, given this URL on a OneNote page: [https://github.com/](https://github.com/)

it would be replaced with its hyperlinked title: [GitHub](https://github.com)

## Sort
Sorts pages, sections, or notebooks. Pages are sorted within the current section only,
not recursively throughout the notebook. Sections are sorted throughout the current
notebook recursively.

> ![Sort](images/SortDialog.png)

## Split Page
Splits the current page at each Heading1 or page links. Also, these can be filtered by an optional tag. 

This will create new pages in the current section. If splitting on page links, if the linked pages exists, it must exist in the current section or it will not be found and a new page will be created in the current section; if it is found then the content will be appended to that page. 

## Strikethrough Completed To Do Tags
Toggles strikethrough text next to all completed/incompleted tags
