## Search and Replace (Ctrl + H)
Searches the current page for the specified phrase and replaces it with a new phrase. Use standard Regular Expression syntax for advanced searches.
Searches line-by-line so it will not find text that spans paragraphs or table cells. If the text cursor is currently within a word, that word is shown as the text to replace.

> ![Search and Replace dialog](images/SearchAndReplace.png)

If the _Replace with_ text contains the string \n then that is replaced with a Newline character.

## Search and Copy/Move (Alt + F)
Searches for keywords across pages and copies or moves selected pages (Alt + F) to another section

> ![Search and Move](images/SearchAndMove.png)

## Tag Page (Alt + T)

Adds one or more arbitrary text tags to a page. Tags can be entered on the fly by typing into the text box. Tags can also be chosen by clicking any from a list of recently used tags or tags inferred from the most commonly occurring words on the page. Enter tags separated with a comma; this allows multi-word tags such as "Wonder Woman".

Tags will appear below the page title, next to the date and time. Note that while this is a block of text that can be edited, that will not change the tags on the page. Page tags must be added, removed, and edited using the Tag Page dialog. Do not modify this text block manually.

> ![Tagging](images/TaggingDialog.png)

## Find Tagged Pages (Ctrl + Alt + T)

Searches pages for the specified page tags. Tags must be separated with a comma. This list of tags is parsed into an inclusion list and an exclusion list where tags are included unless prefaced with a minus operator - such as "-Fish" - these are added to the exclusion list, e.g. "-Fish" will exclude all pages that are tagged with "Fish".

Searching is done by applying both the inclusion list and exclusion list as follows: a page is matched and included in the result list if the page has _one or more of the inclusion tags but none of the exclusion tags_.

You can add tags to the filter by clicking any of the _recently used_ tags; this shows up to 30 tags from the most recently modified pages.

When results are shown, click on each page to force OneNote to navigate to and display that page. 

Select individual pages by ticking the checkbox next to each page. Then create an index page of the selected pages or choose to copy or move those pages to another notebook or another section.

> ![Tagged](images/TaggedDialog.png)


