## Tabs
Tabs make it easy to explore and switch between different views or functional aspects of an app or to browse categorized data sets.

### Usage
1. A tab provides the affordance for displaying grouped content. A tab label succinctly describes the tab’s associated grouping of content.
2. Mobile tabs
3. Desktop tabs
4. When to use
  1. Use tabs to organize content at a high level, for example, presenting different sections of a newspaper. Don’t use tabs for carousels or pagination of content. Those use cases involve viewing content, not navigating between groups of content.
  2. For more detail about using tabs for navigating top-level views, see “Top-level navigation strategies” in Patterns > App structure.
  3. Don't use tabs with content that supports the swipe gesture, because swipe gestures are used for navigating between tabs. For example, avoid using tabs in a map where content is pannable, or a list where items can be dismissed with a swipe.
  4. Fixed tabs should be used with a limited number of tabs and when consistent placement will aid muscle memory. Scrollable tabs should be used when there are many or a variable number of tabs.
5. Tab characteristics
  1. Tabs control the display of content in a consistent location.
  2. Formatting specifications:
    1. Present tabs as a single row. Wrap tab labels to a second line if needed, and then truncate.
    2. Do not include a set of tabbed content within a tab.
    3. Highlight the tab corresponding to the visible content.
    4. Group tabs together hierarchically. Connect a group of tabs with its content.
    5. Keep tabs adjacent to their content. It helps maintain the relationship between the two with less ambiguity.

### Content
1. Content presented in tabs can vary widely, even between tabs. For example, tabs showing different years of an artist’s portfolio or tabs containing different types of settings.
2. All content within a set of tabs should be related under a larger organizing principle (for example, Settings or Directions), with each tab’s content mutually exclusive of the others'.
3. Tab labels should provide meaningful distinctions that logically organize associated content.
4. Tab labels may be either all icons or all text. When choosing a text label, use short titles.
5. Avoid the need for cross-tab comparison of content. Significant cross-tab comparison may indicate the content would benefit from a different organization or presentation that places the content closer together.

### Types of tabs
1. Depending on the platform and the context of use, tabbed content can be presented as either fixed tabs or scrollable (swipeable) tabs.
2. Fixed tabs
  1. Fixed tabs display all tabs concurrently and are best used with content that benefits from quick pivots between tabs in fixed positions, such as switching transportation methods for directions in Google Maps.
  2. Fixed tabs have equal width, calculated either as the view width divided by the number of tabs, or based on the widest tab label. To navigate between fixed tabs, touch the tab or swipe the content area left or right.
3. Scrollable tabs
  1. Scrollable tabs display a subset of tabs at any given moment, and can contain longer tab labels and a larger number of tabs than fixed tabs. Scrollable tabs are best used for browsing contexts in touch interfaces when users don’t need to directly compare the tab labels.
  2. To navigate between scrollable tabs, touch the tab or swipe the content area left or right. To scroll the tabs without navigating, swipe the tabs left or right.

### Specs
1. Fixed tabs
  1. The width of each tab can be calculated by taking the width of the view and dividing it by the number of tabs. Alternatively, make all tabs the width of the largest tab.
  2. If the margin between the tab edge and view edge is 16dp or less, use full-width tabs instead of centered tabs.
  3. Width minimum and maximum (inclusive of padding)
    1. Maximum: 264dp
    2. Minimum: 160dp for larger views, 72 dp for smaller views
  4. Height: 48dp
  5. Padding
    1. 12dp left and right of text
    2. 20dp from bottom for a single line of text, 12dp from bottom for two lines of text
  6. Alignment
    1. Full-width for smaller views
    2. Centered for larger views
  7. Indicator
    1. Height: 2dp
    2. Color: #fff or accent color
2. Tabs with text only
  1. Text
    1. 14sp Roboto Medium
    2. 12sp when wrapped across a maximum of two lines
    3. All caps
    4. Horizontally and vertically centered
    5. Active color: #fff or accent color
    6. Unfocused tab color: #fff 70%
3. Tabs with icons and text
  1. Height: 72dp
  2. Content alignment
    1. Text and icon are centered horizontally in the tab
  3. Padding
    1. 10dp between icon and text
    2. 16dp under text
4. Tabs with icons only
  1. Height: 48dp
  2. Content alignment
    1. Icon is centered horizontally and vertically in the tab
  3. Padding
    1. 12dp under icon
5. Scrollable tabs
  1. The left-most tab content aligns with the keyline. Alignment varies between landscape and portrait to match the different keylines.
  2. The width of each tab is independently calculated.
  3. Width minimum and maximum (inclusive of padding)
    1. Maximum (whichever fits and is smaller): 264dp or (the value of view size minus 56dp)
    2. Minimum: 160dp for larger views, 72 dp for smaller views
  4. Height: 48dp
  5. Padding
    1. 12dp left and right of text
    2. 20dp from bottom for a single line of text, 12dp from bottom for two lines of text
  6. Indicator
    1. Height: 2dp
    2. Color: #fff or accent color
  7. Text
    1. 14sp Roboto Medium
    2. 12sp when wrapped across a maximum of 2 lines
    3. All caps
    4. Vertically and horizontally centered
    5. Active color:  #fff or accent color
    6. Unfocused tab color: #fff 70%
6. Desktop
  1. Width minimum and maximum (inclusive of padding)
    1. Maximum (whichever fits and is smaller): 264dp or (the value of view size minus 56dp)
    2. Minimum: 160dp for larger views, 72 dp for smaller views
  2. Height: 48dp
  3. Alignment
    1. Centered or aligned with left keyline
  4. Text
    1. 13sp Roboto Medium
    2. All caps
    3. Horizontally and vertically centered
    4. Wraps across a maximum of two lines
    5. Active color: #fff or accent color
    6. Unfocused tab color: #fff 70%
  5. Padding
    1. 24dp left and right of text
    2. 20dp from bottom for a single line of text, 12dp from bottom for two lines of text
  6. Indicator
    1. Height: 2dp
    2. Color: #fff or accent color
7. Tab touch target animation
  1. Note: Implementations of this component may vary by platform. By using standard platform implementations, you will receive related future improvements.
