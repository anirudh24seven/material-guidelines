## Progress & activity
Minimize visual changes that occur while your app loads content by representing each operation with a single activity indicator. For example, a refresh operation should display either a refresh bar or an activity circle, but not both.

### Types of indicators
1. When indicators are determinate they indicate how long an operation will take when the percentage complete is detectable.
2. When indicators are indeterminate they request that the user wait while something finishes when it’s not necessary to indicate how long it will take.
3. Both linear and circular progress indicators may be either determinate or indeterminate.
4. Linear
  1. A linear progress indicator should always fill from 0% to 100% and never decrease in value. It should be represented by bars on the edge of a header or sheet that appear and disappear.
  2. For multiple operations happening in sequence, use the indicator to represent the progress as a whole, and not each individual operation.
5. Circular
6. Circular with integration

### Behavior
1. Loading in phases
  1. One-phased loads - Ink (copy and images) loads within an existing, unchanging container.
  2. Two-phased loads - The paper container is generated, then the ink (copy and images) load within it.
  3. Loading content for the first time.
  4. Loading content for the first time.
2. Loading additional content
  1. Example 1: Card expansion - An indeterminate linear indicator is recommended for a card expanding on larger surfaces such as desktop.
  2. Example 2: Scroll up to load more - An indeterminate circular indicator with an initial radial ink reaction is recommended when loading a list from below.
  3. Example 3: Swipe down to refresh - An indeterminate circular indicator with a radial ink reaction is recommended when refreshing a list from above.
