## Adaptive UI

Responsive layouts in material design adapt to any possible screen size. This adaptive UI guidance includes a flexible grid that ensures consistency across layouts, breakpoint details about how content reflows on different screens, and a description of how an app can scale from small to extra-large screens.

### Breakpoints
For optimal user experience, Material user interfaces should adapt layouts for the following breakpoint widths: 480, 600, 840, 960, 1280, 1440, and 1600dp.

1. Summary and detail view content in layouts
  1. Layouts under 600dp wide may fill the screen with a single level of content hierarchy (either summary or detail content, but not both).
  2. Layouts over 600dp wide may place two levels of content hierarchy on the screen (both summary and detail content).
2. Max screen widths
  1. Layouts over 1600dp wide may let the layout grow until it hits a max width. At this point, the grid may do one of the following:
    1. Become center aligned with increased margins
    2. Remain left aligned while the right margin grows
    3. Continue to grow while revealing additional content
3. Breakpoint system
  1. These breakpoints describe column and width specifications for different screens, devices, and orientations. 
  2. For some measurements, the values remain the same even if a device is rotated. For that reason the smallest width in either orientation is the defining value.

### Grid
1. Material design’s adaptive UI is based on a 12-column grid layout. This grid creates visual consistency between layouts, while allowing flexibility across a wide variety of designs. The number of grid columns varies based on the Breakpoint system.
2. Margins and Gutters
  1. The adaptive grid focuses on consistent margin and gutter widths, rather than column width. Material design margins and columns follow an 8dp square baseline grid. Margins and gutters can be 8, 16, 24, or 40dp wide.
  2. Margins and gutters don’t need to be equal. For example, it’s acceptable to use 40dp margins and 24dp gutters in the same layout.
3. Full-width vs Centered
  1. Full-width grids use fluid columns and breakpoints to determine when a layout needs to change.
  2. Centered grids use fixed columns and reflow the layout when all columns (plus a defined margin) no longer fit on screen.
4. Panel Influence on the Grid
  1. As defined in Navigation patterns, the side nav may be permanent, persistent, or temporary. These behaviors apply to any panel, not just a side nav.
  2. Permanent
    1. A permanent panel exists outside of the adaptive grid. The panel appears at a defined breakpoint (when the screen can accommodate the panel) and squeezes content. There are no controls to show/hide the panel.
  3. Side panel effects on the grid - This animation happens in two phases:
    1. A persistent side panel appears, squeezing both content and the grid. Content is accessible while the panel remains visible. The panel hides upon toggling.
    2. A temporary side panel appears, pushing grid content off-screen. Touching either outside the panel, or an item inside the panel, hides the panel.
  4. Temporary Overlay
    1. A temporary panel does not affect the grid or content when off-screen. When toggled to be visible, it can be hidden again by touching anywhere outside the panel or an item inside the panel.
    
### Surface behaviors

When a screen size changes, the UI adapts using the following surface-specific behaviors.

1. Visibility
  1. Permanent - When screen space is available, a surface is always visible.
  2. Persistent - Surface visibility can be toggled between visible and hidden. When visible, interacting with other elements on the screen does not change visibility.
  3. Temporary - Surface visibility can be toggled between visible and hidden. When visible, interacting with other elements on the screen toggles the surface to become hidden or minimized.
  
2. Width
  1. Fixed - Element width stays the same when screen size changes.
  2. Fluid - Element width grows as screen size changes.
  3. Sticky - Element width is fixed until influenced by another element or breakpoint.
  4. Squeeze - Element width contracts as a panel is revealed
  5. Push - Element width stays the same, its position changes horizontally as a panel appears, and it may be partially occluded by a screen’s edge.
  6. Overlay - Element width and position stays the same as a panel appears over content.

3. Descriptors
  1. Above, Below - The y position of an element.
  2. Over, Under - The z position of an element in motion.
  3. In Front, Behind - The static z position of an element.
  4. Left, Right, Centered - The x position of an element
  5. Top, Bottom - The y position of an element and its position relative to a screen edge.
  6. Flat, Raised - The z position, and shadow of an element. A flat element will have no shadow.
  7. Inset, Full Bleed - The padding of an image or element
  8. Summary, Detail - A content summary, and the full expansion of the summary
  
### Patterns

As more screen space is available, the following patterns can be applied.

1. Reveal - Reveal the hidden UI.
2. Transform - UI can transform from one format to another.
3. Divide - Divide UI that was previously layered into newly available space.
4. Reflow - Reflow UI into available space.
5. Expand - Grow the UI to consume more space.
