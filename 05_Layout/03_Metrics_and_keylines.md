## Metrics & keylines

### Baseline grids
All components align to an 8dp square baseline grid. Type aligns to a 4dp baseline grid. Iconography in toolbars align to a 4dp square baseline grid. This applies to mobile, tablet, and desktop.

### Keylines and spacing

1. Mobile
  
  The mobile layout template includes a wide variety of screens and information about how keylines and spacing work across screen edges and elements.
  
  1. List
  2. List with subheadings
  3. Detail view
  4. Mixed content
  5. Navigation drawer

2. Tablet

  The tablet layout template includes 14 different screens and shows how keylines and spacing work across screen edges and elements. 
  
  1. List with detail view
  
3. Desktop

  The desktop layout template includes four different screens, each with four different window sizes, and shows how keylines and spacing work across windows and elements. Based on the window size, the keylines and spacing blocks will inherit grid rules from both tablet and mobile. Here is a sample of a screen available in the download.
  

### Ratio keylines
1. Specific aspect ratios, or the proportion of an element’s width to its height (written as width:height), apply to both UI elements and mobile screen sizing. The following keyline images depict these recommended ratios:
  1. 16:9
  2. 3:2
  3. 4:3
  4. 1:1
  5. 3:4
  6. 2:3
2. Applicable to mobile, tablet, and desktop.
3. For example:
  1. For a 1:1 aspect ratio, an element has equal height and width.
  2. For a 2:3 aspect ratio, an image 360dp wide (full-screen) would have a height of 540.
4. Use one of the aspect ratios above to determine the appropriate width or height of your element:
  1. Width = Aspect ratio * Height
  2. Height = Width/Aspect ratio
  
  (In both formulas, the aspect ratio is expressed as a fraction. For example, 3:2 becomes 3/2, and 16:9 is 16/9).
  
### Incremental keylines
1. An incremental keyline defines an increment, like the height of the action bar, and uses a multiple of that increment to determine the size and position of other elements in the app.
2. Incremental keylines apply mostly to desktop, often to tablet, and rarely to mobile. The number of increments varies based on window size.

### Touch target size
1. To ensure usable apps, touch targets should be at least 48 x 48 dp. In most cases, the space between touch targets should be 8 dp or more.
2. Keep this in mind when spacing icons (24dp) or avatars (40dp) in a layout. The touch targets shouldn’t overlap.
3. On average, 48dp translates to a physical size of about 9mm (with some variability). This is comfortably in the range of recommended target sizes (7-10mm) for touchscreen objects and ensures that users will be able to reliably and accurately target them with their fingers.
4. If you design your elements to be at least 48dp high and wide, you can ensure that:
  1. Your targets won’t be smaller than the minimum recommended target size of 7mm regardless of the screen on which they are displayed.
  2. You strike a good compromise between overall information density and targetability of UI elements.
