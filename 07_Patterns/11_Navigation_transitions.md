## Navigational transitions
1. Navigational transitions are movements between states in an app, such as from a high-level view to a detailed view. Most, but not all, transitions are hierarchical in nature.
2. These moments should reflect the user’s journey through each state of an app appropriately.

### Parent to child
1. Exploring deeper levels, or screens, of an app is a hierarchical journey that starts at a parent screen. From there, a user can explore multiple possible sub-screens, which are children to the parent screen.
2. In material design, elevation changes indicate changes in focus from parent to child elements.
3. Elevation and expansion
  1. The surface that the user touches should lift up and expand into place from its origin. This expansion and motion highlights movement away from the parent towards a destination (a child element) in a natural movement using the material motion curve.

### Sibling to sibling
1. Sibling transitions are transitions that occur between elements at the same level of hierarchy.
2. Static elevation
  1. When a user navigates through tabs, for example, no elevation changes occur. The content and surface of each tab stays at the same elevation level. New content slides in from the right while sibling content moves off-screen to the left.
