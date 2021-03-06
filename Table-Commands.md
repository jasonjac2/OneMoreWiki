## Copy and Fill Commands
The Copy Across and Copy Down commands will duplicate the contents of the lead cells in the selection. For example, if you select one or more cells in the first row and choose Copy Down, the cell values, style, and shading in that row will be copied down the entire table. Restrict the scope by selecting the first cell to copy and subsequent cells to fill, either vertically or horizontally as appropriate.

The Fill Across and Fill Down commands will increment the values in the lead cells in the selection. For example, if the selected cell contains a number, that number will be incremented and added to all subsequent cells. If the second cell is populated then it will compare the second and first cell, determine the difference, and use that to increment the value. The Fill commands work for:

* Numbers including integers, decimals, and currencies, incrementing by 1 or the integer difference of the first and second cell
* Counting Strings such as "Person 1" will be incremented to populated "Person 2", "Person 3", "Person 4", etc.
* Dates of various forms will be recognized and increment by adding 1 day or the different in days between the first and second cell
  * Date formats include these culture-specific formats (change per culture)
    * M/d/YYYY
    * MMMM d
    * dddd, MMM d, yyyy
  * And these specific formats
    * d-MMM-yyyy
    * MMM d, yyyy
    * MMM d

> ![Fill-Down Table](images/FillTable.gif)

## Convert Text to Table
Converts selected text to a table. Text must be delimited by a comma, space, or other special character so the command can detect columns.

## Insert Table Cells
Adds the ability to insert cells into a table, shifting existing content down or to the right.
This is similar to the Excel functionality with one enhancement - if you select a rectangular
region of cells then it will shift just those cells, possibly overwriting other cells. If you
select cells from one column or cells from one row then it will insert cells above or to the left
and add rows or columns as needed to make room for the new cells.

> ![Insert Table Cells](images/InsertCellsDialog.png)

_Note that if you move cells with formulas, the cell references in those formulas are not updated
automatically by this command; you'll need to adjust those manually._

## Paste Table Cells
Paste copied cells into a table, overlaying cells rather than inserting a nested table as OneNote does by default.
The target table is expanded with extra rows or columns as needed. All cell formatting, including cell shading, is preserved.
This is useful for moving cells around within a table or copying cells from one table to another. 

When copying cells with Ctrl-C and pasting back into the same table, the old cells are not erased. If your intention is to _move_ the cells, leaving blank cells behind, then instead use Ctrl-X to copy and cut prior to running this paste command.

Note, you may notice the OneNote windows flashing once when this command is run. This is because OneMore needs to use a temporary page to do some of its work and you're seeing it navigate to that page and then back to your current page.

## Split Table
Splits the current table starting at the row containing the input cursor. Optionally, the header can be duplicated in the new table and columns in both can be fixed to their current widths so the two tables remain aligned.

# Formula Commands

OneNote lets you insert an Excel table on a page or convert a table to an Excel object. This is
convenient if you want complicated formulas and charts... and you have Excel installed! But what
if you don't?

OneMore adds Excel-like formula functionality to native OneNote tables. Thanks to the work done
by [Jonathan Wood](http://www.blackbeltcoder.com/Articles/algorithms/a-c-expression-evaluator),
who created a fantastic expression parser and evaluator, you can apply a formula to one or more
selected cells in a table. A formula can consist of basic mathematical operators, parenthesis,
and most math functions such as abs, sum, average, sin, etc.

| Formula Menu | Formula Dialog |
| ------------ | -------------- |
| ![Formula Menu](images/FormulaMenu.png) | ![Formula Dialog](images/FormulaDialog.png) |

1. Select the cell or cells into which you want to add a formula; they must be linear and
   contiguous, meaning in the same row or in the same column.
1. Select the Add Formula command (F5). The Formula dialog is displayed showing the names of the
   selected cells: A1, A2, A3, etc.
1. Enter the formula. As you type, OneMore validates the syntax in real-time, showing whether
   the formula is valid or invalid. Only when it is valid will the OK button be enabled.
1. Choose the format of the result: Number, Currency, or Percentage.
1. Choose whether you want to tag the cell with a lightning bolt to make it easy to identify
   cells with formulas in them.
1. Click OK.

If you use cell references in your formula and you've selected more than one cell then OneMore
will automatically increment the references relative to each seleted cell. For example, if you
select cells A10, B10, and C10 and enter the formula sum(A1:A9) then that will apply to A10, 
sum(B1:B9) will apply to B10, and sum(C1:C9) will apply to C10.

Formula processing is not recursive. This means that if cell A1 has a formula "A2+1" and cell
A2 has a formula "1+1", then when A1 is calculated, it will not force A2 to be recalculated.
Instead, each cell is calculated in order, top-down and left-to-right across the table.

The Recalculate command (Shift + F5) will recalculate all formulas in the selected table(s).

The Highlight command will select all cells on the page containing formulas so you know where
you put them.

The Delete command will remove a formula from the selected cell(s) but retain the values displayed
in those cell.
