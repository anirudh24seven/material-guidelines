## Lists
Lists present multiple line items in a vertical arrangement as a single continuous element.

### Usage
1. A list consists of a single continuous column of tessellated sub-divisions of equal width called rows that function as containers for tiles.
2. Tiles hold content, and can vary in height within a list.
3. Lists are best suited to presenting a homogeneous data type or sets of data types, such as images and text, optimized for reading comprehension with the goal of differentiating between like data types or qualities within a single data type.
4. If more than three lines of text need to be shown in list tiles, use cards instead.
5. If the primary distinguishing content consists of images, use a grid list.

### Content
1. Tile content
  1. List tiles present collections of related content in a consistent format, using hierarchy to enhance readability by prioritizing a consistent type or set of content. For example, in an email app, an inbox list emphasizes an avatar and text snippet over a time stamp. This helps users more easily find the most important information within the collection of content.
  2. List tiles can contain up to three lines of text, and the amount of text can vary between tiles within the same list. To display more than three lines of text, use a card.
  3. Bias the most distinguishing content in a tile towards the left of the tile. In tiles with mutli-line content, place the most distinguishing content in the first line.
2. Tile actions
  1. The majority of space on a list tile should be dedicated to the primary action.
  2. Because actions are not distinguishing elements of list tiles, place supplemental actions on the right side of the tile.
  3. Primary and supplemental actions, such as play, zoom in, delete, and select, are immediate and typically do not have a submenu of options (action overflow) within the list.
  4. Actions can open a subsequent view, such as a card.
  5. Primary actions:
    1. Fill the entire tile, and therefore are not represented via icons, text, etc.
    2. Are consistent throughout tiles in a specific list. For example, the primary action for all tiles in a single list of music would be to play a song, or in a list of emails, to open an email.
  6. Supplemental actions:
    1. Are represented in tiles with icons, secondary text, etc.
    2. Are functionally consistent throughout tiles in a specific list, for example, an icon that indicates whether someone is online.
    3. Are placed in a consistent location within the tiles of a specific list.
  7. Avoid creating visual noise by repeatedly using supplemental actions in tiles, for example, by displaying a share action in every tile. Toggles, such as stars or pins, are exceptions because they provide meaningful information by displaying a state.
  
### Behavior
1. Scrolling
  1. Lists scroll only vertically.
2. Gestures
  1. Per-tile swipe actions should be consistent within lists.
  2. Where appropriate, tiles can be moved between a list and a drop target (for example, moving a file into a folder) and picked up and manually reordered within a list.
3. Tile filtering and sorting
  1. List tiles can be programmatically sorted or filtered by date, file size, alphabetical order, or other parameters.

### Specs
1. In a single-line list, each tile contains a single line of text. The amount of text can vary between tiles within the same list.
2. In a two-line list, each tile contains a maximum of two lines of text. The amount of text can vary between tiles within the same list.
3. In a three-line list, each tile contains a maximum of three lines of text.
4. The amount of text can vary between tiles within the same list.
5. Single-line list
  1. Text only
    1. Font: Roboto Regular 16sp
    2. Tile height: 48dp
    3. Text padding, top: 16dp
    4. Text padding, bottom: 20dp
    5. Bottom padding is measured from the baseline.
    6. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  2. Icon with text
    1. Font: Roboto Regular 16sp
    2. Tile height: 48dp
    3. Icon padding, left: 16dp
    4. Text padding, left: 72dp
    5. Text padding, top: 16dp
    6. Text padding, bottom: 20dp
    7. Bottom padding is measured from the baseline.
    8. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  3. Icon with text
    1. Font: Roboto Regular 16sp
    2. Tile height: 48dp
    3. Icon padding, left: 16dp
    4. Text padding, left: 72dp
    5. Text padding, top: 16dp
    6. Text padding, bottom: 20dp
    7. Bottom padding is measured from the baseline.
    8. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  4. Avatar with text
    1. Font: Roboto Regular 16sp
    2. Tile height: 56dp
    3. Left avatar padding: 16dp
    4. Text padding, left: 72dp
    5. Text padding, top: 20dp
    6. Text padding, bottom: 24dp
    7. Bottom padding is measured from the baseline.
    8. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  5. Avatar with text and icon
    1. Font: Roboto Regular 16sp
    2. Tile height: 56dp
    3. Left avatar padding: 16dp
    4. Text padding, left: 72dp
    5. Text padding, top: 20dp
    6. Text padding, bottom: 24dp
    7. Bottom padding is measured from the baseline.
    8. Right icon padding: 16dp
    9. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
6. Two-line list
  1. Text only
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp
    3. Tile height: 72dp
    4. Text padding, left: 16dp
    5. Text padding, top and bottom: 20dp
    6. Bottom padding is measured from the baseline.
    7. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding
  2. Icon with text
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp
    3. Tile height: 72dp
    4. Left icon padding: 16dp
    5. Text padding, left: 72dp
    6. Text padding, top and bottom: 20dp
    7. Bottom padding is measured from the baseline.
    8. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  3. Avatar with text
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp
    3. Tile height: 72dp
    4. Left avatar padding: 16dp
    5. Text padding, left: 72dp
    6. Text padding, top and bottom: 20dp
    7. Bottom padding is measured from the baseline.
    8. Center-align icon with text area.
    9. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  4. Avatar with text and icon
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp
    3. Tile height: 72dp
    4. Left avatar padding: 16dp
    5. Text padding, left: 72dp
    6. Text padding, top and bottom: 20dp
    7. Bottom padding is measured from the baseline.
    8. Right icon padding: 16dp
    9. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
3. Three-line list
  1. Text only
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp
    3. Tile height: 88dp
    4. Text padding, left: 16dp
    5. Text padding, top: 16dp
    6. Text padding, bottom: 20dp
    7. Bottom padding is measured from the baseline.
    8. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  2. Icon with text
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp 
    3.Tile height: 88dp
    4. Left icon padding: 16dp
    5. Text left padding: 72dp
    6. Text padding, top: 16dp
    7. Text padding, bottom: 20dp
    8. Bottom padding is measured from the baseline.
    9. Top-align icon with primary text.
    10. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  3. Avatar with text
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp
    3. Tile height: 88dp
    4. Left avatar padding: 16dp
    5. Left text padding: 72dp
    6. Text padding, top: 16dp
    7. Text padding, bottom: 20dp
    8. Bottom padding is measured from the baseline.
    9. Top-align avatar with primary text.
    10. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
  4. Avatar with text and icon
    1. Primary text font: Roboto Regular 16sp
    2. Secondary text font: Roboto Regular 14sp
    3. Tile height: 88dp
    4. Left avatar padding: 16dp
    5. Text left padding: 72dp
    6. Text padding, top: 16dp
    7. Text padding, bottom: 20dp
    8. Bottom padding is measured from the baseline.
    9. Right icon padding: 16dp
    10. Top-align avatar and icon with primary text.
    11. Add 8dp padding at the top and bottom of a list. One exception is at the top of a list with a subheader, because subheaders contain their own padding.
