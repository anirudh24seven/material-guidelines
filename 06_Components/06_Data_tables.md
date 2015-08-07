## Data tables
1. Data tables are used to present raw data sets, and usually appear in desktop enterprise products.
2. Data sets may include:
  1. Three or more columns of data
  2. A corresponding visualization
  3. The ability for users to query and manipulate data at scale
  
### Structure
In its simplest form, a data table contains a top row of column names, and rows for data. Checkboxes should accompany each row if the user needs to select or manipulate data.

1. Column headers
  1. 12sp Roboto Medium
  2. 54% black
2. Table content
  1. 13sp Roboto Regular
  2. 87% black
3. Text alignment
  1. Right-align numeric columns
  2. Left-align text columns

### Interaction
1.Row hover (Desktop)
  1. Display a background fill when the user hovers over any part of a row. If there are separate hover states on individual (e.g. editable) cells, display both the hover state of the cell and row at the same time.
  2. Hover background - Grey 200 (#EEEEEE)
2. Row selection
  1. When a row is selected, use a background fill on the row.
  2. Selected row background
    1. Grey 100 (#F5F5F5)
  3. Checkbox
    1. Use secondary app color
3. Sorted column
  1. If column sorting is enabled, sort the most important data by default and display a sorted state in the column header. If the user clicks on a column that is already sorted, reverse the sort order and rotate the sort icon.
  2. Sorted column name
    1. 12sp Roboto Medium
    2. 87% black
  3. Sort icon
    1. 16dp container
    2. 87% black
4. Column name hover (Desktop)
  1. If there is a need to provide definitions to column headers, display a tooltip on hover. If sorting is enabled, display a light sort icon upon hover, which indicates that the column is sortable.
  2. Tooltip
    1. Follow the guidelines for Tooltips
  3. Sort icon
    1. 16dp container
    2. 26% black
5. Long header titles
  1. Sometimes, column names don’t fit in a container with the recommended 56dp of padding in between columns. There are two options to handle this:
    1. Display the full column name and enable horizontal scrolling in the table container.
    2. Shorten the column name and display it in full on hover.
6. Inline text editing
  1. Tables may require basic text editing (e.g. for editing existing text content, or adding comments). Include editable fields within a table and denote them using placeholder text. You can use a simple edit dialog with just a text field, or display a full dialog component on click.
  2. Placeholder text
    1. 13sp Roboto Regular
    2. 26% black
    3. No divider line on text field
  3. Small edit dialog
    1. Align edges of dialog with nearest divider lines, or table edges
    2. 24dp of left and right padding
    3. Include a single text field, applying the app theme where applicable
    4. User confirms text by pressing Enter
  4. Large edit dialog
    1. Align edges of dialog with nearest divider lines, or table edges
    2. Follow the dialog guidelines, applying the app theme where applicable
    3. User confirms text by clicking the Save button
  5. Inline edit icon
    1. 18dp container
    2. 54% black
7. Inline menus
  1. Instead of editing text, users may need to select from a predefined list of options. In this scenario, embed a menu component directly in the table.
  2. Inline menu
    1. 13sp Roboto Regular
    2. 87% black
    3. Follow spacing and sizing guidelines for menus
    
### Tables within cards
1. Tables can be embedded within a card, with table navigation and data manipulation tools available at the top and bottom.
2. Card title
  1. 20sp Roboto Regular
  2. 87% black
3. Card action icons (header and footer)
  1. 24dp container
  2. 54% black
4. Footer pagination labels
  1. 12sp Roboto Regular
  2. 54% black
5. Alternate headers
  1. Some table cards may require headers with actions instead of titles. Two possible approaches to this are to display persistent actions, or a contextual header that activates when items are selected.
  2. Action buttons
    1. Use borderless buttons
    2. Enable upon item selection
  3. Colored header
    1. Use 50-value of secondary app color for background fill
    2. Display the number of items selected
    3. Display available contextual icons upon item selection
  
### Specs
1. Vertical spacing
  1. 64dp card header height
  2. 56dp height for last row
  3. 48dp data row height
2. Header & footer padding
  1. 24dp of padding around the perimeter of table cards
  2. 32dp in between footer control sets
  3. 40dp in between the footer row count and its label
3. Column padding
  1. Use a minimum of 56dp of padding in between columns. The widest item in the column (including data and column name) should delineate the column border.
  2. Checkbox icons have a width and height of 18dp within a 24dp icon container.
