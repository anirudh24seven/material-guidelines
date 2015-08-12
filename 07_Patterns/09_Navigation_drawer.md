## Navigation drawer

The navigation drawer slides in from the left. It is a common pattern found in Google apps and follows the keylines and metrics for lists.

### Specs
1. Typography
  1. Name: Roboto Medium, 14sp, #FFFFFF
  2. Email address: Roboto Regular, 14sp, #FFFFFF
  3. List item: Roboto Medium, 14sp, 87% #000000
  4. Subheader: Roboto Medium, 14sp, 54% #000000. Aligns to the 16dp keyline.
2. Keylines and margins
  1. Icons align at screen left and right margins: 16dp
  2. Icon values: 54% #000000
  3. Content associated with an icon or avatar left margin: 72dp
  4. Side nav width: Equal to the screen width minus the height of the action bar. In the example shown this is 56dp from the right edge of the screen. The maximum width of the nav drawer is five times the standard increment (56dp on mobile and 64dp on tablet).
  5. Use 16dp horizontal margins on mobile and 24dp on tablet
3. Vertical spacing
  1. Status bar: 24dp
  2. Subtitle: 56dp
  3. Space between content areas: 8dp
  4. Subtitles and list items: 48dp
  5. Add 8dp padding at the top and bottom of every list grouping. One exception is at the top of a list with a subheader, because subheaders contain their own padding.

### Content
1. Elevation
  1. The nav drawer spans the full height of the screen, including behind the status bar. Everything behind the drawer is still visible but darkened by a scrim.
2. Selection state
  1. After a list item is selected, that item changes color to match the app’s primary color (or #000000 100%) to indicate selection. Additionally, the touch ripple highlights the row of that list item.
  2. If the color of the touch ripple/highlight doesn’t contrast enough with your primary color, use a darker tint of the primary color.
3. Dividers
  1. All dividers in the nav drawer are full-bleed within the drawer, 8dp padding above and below each divider.
4. Scrolling
  1. The navigation drawer scrolls in the same way a view scrolls.
5. Settings and support
  1. Settings and support are located at the bottom of the scrolling list, inline with the rest of the list content. They refer to Help, Feedback, or Help & feedback, depending on what your product offers.

### Behavior
1. Permanent
  1. Recommended default for desktop
  2. Permanent navigation drawers are always visible and pinned to the left edge, at the same elevation as the content or background. They cannot be closed.
  3. The threshold for pinning is calculated using these minimum values:
    1. Side nav width
    2. Content width
    3. Content padding
  4. Types of permanent navigation drawers - The structure and behavior of the overall interface determines which type of permanent navigation drawer to use:
    1. Full-height navigation drawer: Apps focused on information consumption that use a left-to-right hierarchy
    2. Navigation drawer clipped under the app bar: Apps focused on productivity that require balance across the screen
    3. Floating navigation drawer: Apps that require less hierarchy
2. Persistent
  1. Persistent navigation drawers can toggle open or closed. The drawer sits on the same surface elevation as the content. It is closed by default and opens by selecting the menu icon, and stays open until closed by the user. The state of the drawer is remembered from action to action and session to session.
  2. Sitting outside of the page grid, when opened the drawer forces other content to change size and adapt to the smaller viewport.
  3. Persistent navigation drawers are acceptable for all sizes larger than mobile.
  4. Persistent navigation drawers are not recommended for apps with multiple levels of hierarchy that require using an up arrow for navigation.
3. Mini variant
  1. In this variation, the persistent navigation drawer changes its width. Its resting state is as a mini-drawer at the same elevation as the content, clipped by the app bar. When expanded, it appears as the standard persistent navigation drawer.
  2. Recommended for: .Apps sections that need quick selection access alongside content
4. Temporary
  1. Temporary navigation drawers can toggle open or closed. Closed by default, the drawer opens temporarily above all other content until a section is selected.
  2. Recommended for: Tablet
  3. Required for: Mobile
  4. The mini variant is also an acceptable closed state for a temporary navigation drawer.

