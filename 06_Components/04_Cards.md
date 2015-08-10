## Cards
1. A card is a piece of paper with unique related data that serves as an entry point to more detailed information. For example, a card could contain a photo, text, and a link about a single subject.
2. Cards have a constant width and variable height. The maximum height is limited to the height of the available space on a platform, but it can temporarily expand (for example, to display a comment field). Cards do not flip over to reveal information on the back.

### Usage
1. Definition
  1. Cards are a convenient means of displaying content composed of different elements. They’re also well-suited for showcasing elements whose size or supported actions vary, like photos with captions of variable length.
  2. A card collection is coplanar, or a layout of cards on the same plane.
2. When to use - Use a card layout when displaying content that:
  1. As a collection, comprises multiple data types (for example, the card collection consists of images, movies, and text).
  2. Does not require direct comparison (a user is not directly comparing images or text strings).
  3. Supports content of highly variable length, such as comments.
  4. Consists of rich content or interaction, such as +1 buttons or comments.
  5. Would otherwise be in a list but needs to display more than three lines of text.
  6. Would otherwise be in a grid list but needs to display more text to supplement the image.
  
### Content
1. Card content type and quantity can vary greatly. Cards within a card collection can each contain a unique data set. For example, various cards within a card collection might contain a checklist with an action, a note with an action, and a note with a photo.
2. Cards provide context and an entry point to more robust information and views. Don't overload cards with extraneous information or actions.
3. Content hierarchy
  1. Use hierarchy within the card to direct users’ attention to the most important information. For example, place primary content at the top of the card, or use typography to emphasize primary content.
4. Images can help users easily compare and contrast content between cards. However, their size and placement within the card depends on whether images are the primary content or being used to supplement other content on the card.
5. Background images
  1. Text is most legible when placed on a solid color background with a sufficient contrast ratio to the text. Text placed on image backgrounds should preserve text legibility.
  
### Actions
1. The primary action in a card is typically the card itself.
2. Supplemental actions can vary from card to card in a collection, depending on the content type and expected outcome; for example, playing a movie versus opening a book. Within cards in a collection, position actions consistently.
3. Supplemental actions
  1. Supplemental actions within the card are explicitly called out using icons, text, and UI controls, typically placed at the bottom of the card.
  2. Limit supplemental actions to two actions, in addition to an overflow menu.
4. UI controls
  1. UI controls, like a slider, placed inline with primary content can modify the view of the primary content. For example, a slider to choose a day, stars to rate content, or a segmented button to select a date range.
5. Overflow menu
  1. An overflow menu (optional) is typically placed in the upper-right corner of cards, but can be in the lower right if the placement improves content layout and legibility.
  2. Take care not to overload an overflow menu with too many actions.
6. Considerations
  1. Inline links within text content are strongly discouraged.
  2. Although cards can support multiple actions, UI controls, and an overflow menu, use restraint and remember that cards are entry points to more complex and detailed information.
  
### Content blocks
1. Cards are constructed using blocks of content which include:
  1. An optional header
  2. A primary title
  3. Rich media
  4. Supporting text
  5. Actions
2. These content blocks can be combined to create visual hierarchy within a card.
3. Content block types
  1. Rich media
    1. 16:9 or 1:1 aspect ratio (recommended)
  2. Actions
    1. Padding: 8dp  
  3. Primary title/text
    1. Title: 24sp or 14sp
    2. Subtitle: 14sp
    3. Left and right padding: 16dp
    4. Top padding: 16dp or 24dp (when a large primary title is present)
    5. Bottom padding: 16dp (if there are additional actions or supporting text) or 24dp (no actions or supporting text)
  4. Supporting text
    1. Supporting text: 14sp
    2. Left and right padding: 16dp
    3. Top padding: 16dp
    4. Bottom padding: 24dp (16dp if there are additional actions or text below)
    5. Bullet points (but not their text), images, and buttons may extend outside of the 16dp padding.
  5. Card margins on mobile
    1. Padding from edge of screen to card: 8dp
    2. Space between cards: 8dp
  6. Elevation
    1. Card resting elevation: 2dp
    2. Card raised elevation: 8dp
4. Content block combinations
  1. The following examples illustrate some possible combinations of content blocks.
    1. Example 1
      1. Media area - 16:9 ratio
      3. Supporting text
        1. Text: 14sp
        2. Padding: 16dp
    2. Example 2
      1. Avatar, Title, and Subtitle area - 72dp
      2. Media area - 16:9 ratio
      3. Supporting text
        1. Text: 14sp
        2. Padding: 16dp
      4. Actions - Padding: 8dp
    3. Example 3
      1. Avatar, Title, and Subtitle area - 72dp
      2. Media area - 16:9 ratio
      3. Actions
        1. Padding: 8dp
        2. Padding between actions: 4dp
    4. Example 4
      1. Media area - 16:9 ratio
      2. Primary text
        1. Text: 24sp
        2. Top padding: 24dp
        3. Bottom padding: 16dp
      3. Subtext
        1. Text: 14sp
        2. Bottom padding: 16dp
      4. Actions - Padding: 8dp
    5. Example 5
      1. Media area - 16:9 ratio
      2. Primary text
        1. Text: 24sp
        2. Top padding: 24dp
        3. Bottom padding: 16dp
      3. Subtext
        1. Text: 14sp
        2. Bottom padding: 16dp
      4. Actions - Padding: 8dp
      5. Expanded supporting text
        1. Text: 14sp
        2. Top padding: 16dp
        3. Bottom padding: 24dp
    6. Example 6
      1. Primary text
        1. Text: 24sp
        2. Top padding: 24dp
        3. Bottom padding: 16dp
      2. Subtext
        1. Text: 14sp
        2. Bottom padding: 16dp
      3. Supporting text
        1. Text: 14sp
        2. Top padding: 16dp
        3. Bottom padding: 16dp
      4. Actions - Padding: 8dp
    7. Example 7
      1. Media area - 16:9 ratio
      2. Actions - Padding: 8dp
    8. Example 8
      1. Media area - 1:1 ratio
      2. Primary text
        1. Text: 24sp
        2. Top padding: 24dp
      3. Subtext
        1. Text: 14sp
        2. Bottom padding: 16dp
      4. Actions - Padding: 8dp 
    9. Example 9
      1. Media area - 1:1 ratio
      2. Primary text - Text: 24sp
      3. Actions - Padding: 8dp
    10. Example 10
      1. Media area
        1. 1x
        2. Top padding: 16dp
      2. Primary text
        1. Text: 24sp
        2. Top padding: 24dp
      3. Subtext - Text: 14sp
      4. Actions - Padding: 8dp 
    11. Example 11
      1. Media area
        1. 3/8x
        2. Top padding: 16dp
      2. Primary text
        1. Text: 24sp
        2. Top padding: 24dp
      3. Subtext - Text: 14sp
      4. Actions - Padding: 8dp
    12. Example 12
      1. Media area
        1. 2x
        2. Top padding: 16dp
      2. Primary text
        1. Text: 24sp
        2. Top padding: 24dp
      3. Subtext - Text: 14sp
      4. Actions - Padding: 8dp 
    13. Example 13
      1. Media area
        1. 3x
        2. Padding: 16dp
      2. Actions - All around padding: 8dp + 16dp 
  

### Behavior
1. Supported gestures
  1. The swipe gesture is supported on a per-card basis. Card gestures should be consistently implemented within a card collection.
  2. Limit swipe gestures within a view so that they don’t overlap with one another. For example, a swipeable card should not contain a swipeable image carousel so that only a single action occurs when the card is swiped.
  3. The pick-up-and-move gesture is also supported. However, consider whether it is important for the user to be able to sort cards within the collection, or if the content would be better organized using programmatic filtering or sorting.
2. Card collection filtering and sorting
  1. Card collections can be programmatically sorted or filtered by date, file size, alphabetical order, or other parameters. The first item in the collection is positioned at the top left of the collection, and the order proceeds left to right and top to bottom.
3. Scrolling
  1. Card collections only scroll vertically. Card content that exceeds the maximum card height is truncated and does not scroll.
  2. Cards with truncated content can be expanded, which means the card height may exceed the maximum height of the view. In this case, the card will scroll with the card collection. 
4. Card focus
  1. When traversing through focus points on a card, all focusable elements are visited before moving to the next card.
  2. For interfaces that depend on focus traversal for navigation (D-pad and keyboard), cards should have either a primary action or open a new view containing primary and supplemental actions.
