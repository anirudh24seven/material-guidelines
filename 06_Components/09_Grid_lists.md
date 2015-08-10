## Grid lists
Grid lists are an alternative to standard list views. Grid lists are distinct from grids used for layouts and other visual presentations.

### Usage
1. A grid list is best suited to presenting homogenous data, typically images, and is optimized for visual comprehension and differentiating between similar data types.
2. A grid list consists of a repeated pattern of cells arrayed vertically and horizontally within the grid list.
3. Tiles hold content and can span one or more cells vertically or horizontally.
4. If the text in tiles needs to be prominent enough to distinguish between primary content pieces, consider using a different container, like a list or cards, optimized for displaying text and facilitating reading comprehension.
5. Lists: Optimized for reading comprehension, particularly when comparing a set of data containing multiple data types.
6. Cards: Used for content with inconsistent formatting, such as photos with captions of variable length, or data sets with heterogeneous content, such as a mixed collection of photos and videos and books.

### Content
1. Content in tiles
  1. Tile content consists of primary content and secondary content. Primary content is the main differentiating element, typically an image. Secondary content can be an action or text.
  2. Provide a default image for tiles that lack an image for primary content.
2. Actions in tiles
  1. Actions on both primary and secondary content—such as play, zoom in, delete, or select—are immediate and typically do not result in a submenu of options (action overflow) within the grid list.
  2. Actions can open a subsequent view, such as a card.
  3. Primary actions
    1. Fill the entire tile and therefore are not represented via icons or text.
    2. Are consistent throughout tiles in a specific grid list. For example, the primary action for all tiles in a single grid list could be to view details for an image.
  4. Secondary actions or content
    1. Are represented in tiles with icons or text.
    2. Are consistent throughout tiles in a specific grid list.
    3. Are placed in a consistent location within the tiles of a specific grid list, but that consistent location may vary between grid lists (at corners or edges). For example, all titles in one grid list could be located at the bottom left corner, while all tiles in another grid list might place titles in the top left corner.

### Behavior
1. Scrolling
  1. Grid lists typically scroll only vertically.
  2. Horizontally scrolling grid lists are discouraged because the scrolling interferes with typical reading patterns, affecting comprehension. One notable exception is a horizontally-scrolling, single-line grid list of images, such as a gallery, which is compatible with typical reading patterns.
  3. Cut off grid tiles in the view’s initial scroll position to communicate the scroll direction for content overflow.
2. Gestures
  1. Per-tile swipe actions are not permitted. Pick-up-and-move actions are discouraged.
3. Tile filtering and sorting
  1. Content in a grid list can be programmatically filtered or sorted by date, file size, alphabetical order, or other parameters.
  2. The first item in the grid list is positioned at the top left of the grid list, and the order proceeds left to right and top to bottom.
4. Dimensions and resizing
  1. Resizing a grid list causes the tiles to re-sort as horizontal space becomes available. Full-bleed grid list tiles resize to fit the screen width.
  2. A grid list does not transform into a list when horizontal space contracts. Grid lists and lists are separate structures for emphasizing different data types. Grid lists prioritize images over text and lists prioritize text over images.
  3. To maintain a consistent rhythm throughout the grid list, truncate text content that is too long for the tile’s width. Alternatively, increase the grid size so that the tiles can accommodate the longer titles.
5. Responsive design
  1. Full-screen grid lists should use fluid image ratios with minimum and maximum widths, derived using the Ratio keylines. They should retain fixed heights, margins, and padding.
  2. Centered grid lists have fluid margins with a minimum width. They maintain fixed image widths, heights, and padding.
  
### Specs
1. Grid list header/footers
  1. Single-line header/footer
    1. Height: 48dp
    2. Text padding: 16dp
    3. Default font size: 16sp
    4. Secondary action is flush right to the footer.
  2. Two-line header/footer
    1. Height: 68dp
    2. Text padding: 16dp
    3. Default font size for each line: 16sp/12sp or 14sp/14sp
2. Image-only grid list
  1. Grid list padding: 4dp or 1dp
  2. Tiles in grid lists can span multiple columns.
  3. Carefully consider whether secondary text is needed in grid lists that use multi-column tiles, as larger tiles can develop significant empty space.
3. Single-line grid list
  1. Text only
    1. Height: 48dp
    2. Text padding: 16dp
    3. Default font size: 16sp
    4. Grid list padding: 4dp or 1dp
  2. Text with icon
    1. Height: 48dp
    2. Text padding: 16dp
    3. Default font size: 16sp
    4. Grid list padding: 4dp or 1dp
    5. The secondary action can be flush right or flush left within the footer or header.
4. Two-line grid list
  1. Text only
    1. Height: 68dp
    2. Text padding: 16dp
    3. Default font size for each line: 16sp/12sp or 14sp/14sp
    4. Grid list padding: 4dp or 1dp
