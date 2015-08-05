## Structure

### UI regions
1. Mobile structure
  1. This structure includes a permanent app bar and floating action button. An optional bottom bar can be added for additional functionality or action overflow. Side nav menus overlay all other structural elements.
2. Tablet structure
  1. This structure shows a permanent app bar with a floating action button. The app bar absorbs elements from the tablet and mobile bottom bars. An optional bottom bar can be added for additional functionality or action overflow. A side nav overlays all other structural elements. A right nav menu can be accessed temporarily or pinned for permanent display.  
3. Desktop structure
  1. The desktop structure contains a permanent app bar with a floating action button. The app bar absorbs elements from the tablet and mobile bottom bars. Where possible, the window controls are absorbed into the app bar.
  2. Side navigation menus can take up the full height of the screen size (including under the app bar) and be accessed temporarily or pinned for permanent display. Side nav menus, as well as the content canvas, can have their own secondary toolbars for tabs, palettes, or secondary actions.  
4. UI regions
  1. Define a primary horizontal or vertical divider.
  2. Avoid slicing up the interface into too many regions which can cause L shapes. Instead, use whitespace to delineate secondary areas.
  3. Break edges with cards and floating action buttons.
  4. Use cards to organize content when specific behaviors are needed or if groupings of information need more separation than what whitespace or dividers can provide.
  
### Toolbars
1. Toolbars are versatile and can be used in many different ways. 
2. Here are some examples:
  1. Full-width, default height app bar
  2. Full-width, extended height app bar
  3. Column-width toolbars at multiple levels of hierarchy
  4. Flexible toolbar and card toolbar
  5. Floating toolbar
  6. Detached toolbar palette
  7. Bottom toolbar that launches to a shelf and clings to the top of the keyboard or other bottom component
  8. Bottom toolbar shelf
  
### App bar
1. The app bar, formerly known as the action bar in Android, is a special kind of toolbar that’s used for branding, navigation, search, and actions.
2. The nav icon at the left side of the app bar can be:
  1. A control to open a navigation drawer.
  2. An up arrow for navigating upward through your app’s hierarchy.
  3. Omitted entirely if no navigation is required from this screen.
3. The title in the app bar reflects the current page. It can be an app title, page title, or a page filter.
4. Icons on the right side of the app bar are app-related actions. The menu icon opens the overflow menu, which contains secondary actions and menu items like help, settings, and feedback.
5. Title color
  1. In an app bar, all icons should be the same color.
  2. The title can have a distinct color from the icons if increased visual hierarchy is needed. Distinct title colors work best on backgrounds with enough contrast for both white and black glyphs.
6. Metrics - Default heights:
  1. Mobile Landscape: 48dp
  2. Mobile Portrait: 56dp
  3. Tablet/Desktop: 64dp
  4. For extended app bars, the height is equal to the default height plus content increment(s).
7. Menus
  1. A menu is a temporary sheet of paper that always overlaps the App Bar, rather than behaving as an extension of the App Bar.
  
### System bars
1. Status bar/window bar
  1. On Android, the status bar contains notification icons and system icons. On Chrome, the top bar contains the window controls: minimize, full screen, and close. In a Chrome app, the top bar can disappear, and the window controls are then brought into the app bar.
  2. Metrics:
    1. Android status bar height: 24dp
    2. Chrome window height: 32dp
2. Dark status bar
  1. By default, the color of the status or window bar is a darker shade of the app bar color. It can also use color from another element in the layout or be translucent.
3. Light status bar
  1. The light status bar, with dark icons, better harmonizes with light content and can be used an alternative to the dark status bar.
4. Android navigation bar
  1. The navigation bar in Android houses the device navigation controls: Back, Home, and Overview. It also displays a menu for apps written for Android 2.3 or earlier.
  2. Height: 48dp
  3. Color variants: The navigation bar can be opaque, translucent, or transparent.
5. Chrome OS shelf
  1. The shelf houses the app launcher, application icons, and system settings on Chrome OS.
  2. Height: 56dp
  
### Side nav
1. If present, side nav bars can be pinned for permanent display or float temporarily as overlays. Side navs can be positioned on the left or right side of the screen.
2. The content appearing in the left nav is ideally navigation- or identity-based. Right nav content should be secondary to the main content on a page.
3. Structure
  1. Side nav bars may be pinned for permanent display, or they can float temporarily as overlays. Temporary nav drawers overlay the content canvas; whereas pinned nav panels are situated alongside or below the content canvas.
  2. Screen size can determine whether a panel is pinned or an overlay. With sufficient space, a panel can be pinned and content adjusted responsively. With insufficient space, a panel has to be an overlay.
4. Metrics
  1. Mobile:
    1. Width = Screen width − 56 dp
    2. Maximum width: 320dp
    3. Maximum width applies only when using a left nav. When using a right nav, the panel can cover the full width of the screen.
  2. Desktop: Maximum width for a left nav is 400dp. The right nav can vary depending on content.


### White frames

Whiteframes provide a variety of layout structures using a consistent approach to surfaces, layering, and shadows.

1. Carded content that expands and collapses
2. Overlayed content details with focused app bar on mobile
3. Overlapping content card with multiple toolbars and background image on mobile
4. Extended app bar and right side nav
5. Left side nav and one-up stream on mobile
6. Source list
7. Full-screen background image with inset search field and carded search results
8. Expandable footer drawer

