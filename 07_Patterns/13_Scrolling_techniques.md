## Scrolling techniques

### Scrolling
1. Scrollable regions
  1. When designing scrolling behavior, app bars contain four main regions (referred to as blocks) that comprise the scrolling structure:
    1. Status bar
    2. Tool bar
    3. Tab bar/search bar
    4. Flexible space: space to accommodate a desired aspect ratio for images or extended app bars
2. Standard app bar
  1. The standard app bar height is 56dp on mobile and 64dp on larger screen sizes.
  2. There are two options for scrolling:
    1. The app bar can scroll off-screen with the content and return when the user reverse scrolls.
    2. The app bar can stay fixed at the top with content scrolling under it.
3. Tabs
  1. The standard app bar is the overarching component that can include the following blocks: a toolbar, tab bar, or flexible space.
  2. It can have one of the following behaviors:
    1. The tab bar stays anchored at the top, while the toolbar scrolls off.
    2. The app bar stays anchored at the top, with the content scrolling underneath.
    3. Both the toolbar and tab bar scroll off with content. The tab bar returns on reverse-scroll, and the toolbar returns on complete reverse scroll.
4. Flexible space
  1. Because the app bar is flexible, it can be extended to accommodate larger typography or images. To extend the app bar, add a flexible space block.
  2. There are two display options:
    1. The flexible space shrinks until only the toolbar remains. The title shrinks to 20sp in the navigation bar. When scrolling to the top of the page, the flexible space and the title grow into place again.
    2. The whole app bar scrolls off. When the user reverse scrolls, the toolbar returns anchored to the top. When scrolling all the way back, the flexible space and the title grow into place again.
5. Flexible space with image
  1. Use flexible space to accommodate images in the app bar with the desired aspect ratio.
  2. In this example, the aspect ratio is 4:3. When scrolling, the content pushes up the image, which shrinks the flexible space. At the end of the transformation, the image gets tinted with the primary color, independent of scrolling.
6. Flexible space with overlapping content
  1. Content can overlap the app bar.
  2. Behavior: The app bar’s starting position should be located behind the content. Upon upward scroll, the app bar should scroll faster than the content, until the content no longer overlaps it. Once anchored in place, the app bar lifts up to allow content to scroll underneath.
  3. In this interaction, the app bar cannot include tabs.
