## Buttons: Floating Action Button

### Floating action button
1. Floating action buttons are used for a promoted action. They are distinguished by a circled icon floating above the UI and have motion behaviors that include morphing, launching, and a transferring anchor point.
2. Floating action buttons come in two sizes:
  1. Default size: For most use cases
  2. Mini size: Only used to create visual continuity with other screen elements
3. The floating action button should be placed 16dp minimum from the edge on mobile and 24dp minimum on tablet/desktop.
4. The floating action button has an ink wash upon focus and lifts upon being selected.
5. Not every screen needs a floating action button. A floating action button represents the primary action in an application.
6. Only one floating action button is recommended per screen to increase its prominence. It should represent only the most common action.

### Qualities: 
1. Make floating action buttons positive actions like Create, Favorite, Share, Navigate, and Explore.
2. Avoid using floating action buttons for minor and destructive actions, including the following:
  1. Archive or Trash
  2. Nonspecific actions
  3. Alerts or errors
  4. Limited tasks like cutting text
  5. Controls that should be in a toolbar, like volume control or changing a font color
3. Floating action buttons don’t contain app bar icons or status bar notifications. Don’t layer badges or other elements over a floating action button.
4. Use the circle-shaped icon consistently to enforce the primary action pattern across apps.
5. Don’t give the floating action button extra dimension.

### Behavior
1. The floating action button animates onto the screen as an expanding piece of material, by default. The icon within it may be animated.
2. Floating action buttons may appear and move on screen differently than other UI elements because of their relative importance. Consider the order of elements appearing and how the floating action button fits into that order.
3. If there is a floating action button on multiple lateral screens (such as on tabs), upon entering each screen, the button should show and hide if the action contained on each is different. If the action is the same, the button should stay on screen (and translate to a new position, if necessary.)
4. For tabbed screens, the floating action button should not exit the screen in the same direction as the screen exits. Doing so creates visual noise. It would also cause a nonfunctional floating action button to appear on screen. Furthermore, it incorrectly implies that the floating action button is at the same the z-level as the content, rather than at the level of the primary UI elements at the root level.

### Transitions
1. Transitions
  1. The floating action button is a unique example of a primary use case in an app. Take advantage of its visibility to create delightful transitions for a primary UI element.
  2. Common transitions include Trigger, Toolbar, Speed dial, and Morphing. This is not an exhaustive list. Floating action buttons are designed to be flexible. Experiment with transitions that best suit your app and the screens on which the button sits.
2. Trigger
  1. The floating action button can simply trigger an action or navigate somewhere. The animation of the touch ripple expands outwards as the force that causes changes to the UI.
3. Toolbar
  1. The floating action button can transform into a toolbar upon press or from a toolbar upon scroll. The toolbar can contain related actions, text and search fields, or any other items that would be useful at hand.
  2. A toolbar that disappears on scroll is particularly useful for screens where the full toolbar is needed upon initial entry or while at the top or bottom of a long list. This saves screen real estate when the user has signaled through scrolling that they’re interested in looking at the main content.
  3. If a floating action button morphs into a toolbar, that toolbar should contain related actions.
4. Speed dial
  1. The floating action button can fling out related actions upon press. The button should remain on screen after the menu is invoked. Tapping in the same spot should either activate the most commonly used action or close the open menu.
  2. The floating action button can transform into a single sheet of material which contains all the actions.
  3. As a general rule, have at least three options upon press but not more than six, including the original floating action button target. If you have two options—i.e. your floating action button only flings out one other choice —choose which action is most important. If you have more than six, users may have trouble reaching the furthest option.
  4. Reduce decision fatigue by giving users the best, most distinct, and fewest options.
  5. Don’t put overflow menus in the floating action button actions. There should be at most two taps from the initial screen to get to the intended destination.
  6. Put overflow actions in the overflow menu in toolbars, not in floating action buttons.
  7. If the hallmark of the app is adding file types, a floating action button can transform into related actions after it is first touched. However, if the actions that appear are unrelated to the button, place the actions into an overflow menu.
  8. A floating action button can contain a list of contacts. The list shouldn’t contain unrelated actions.
5. Morph
  1. The floating action button can transform into sheets of material that are part of the app structure. This dramatic transformation accentuates the action the button enables.
  2. When morphing the floating action button, transition between starting and ending positions in a logical way. For example, do not pass through other sheets of material.
  3. The morph animation should be reversible and transform the new sheet of material back into the floating action button.
6. Full screen
  1. The floating action button can transform into a new sheet of material that spans the entire screen.
  2. This type of dramatic transformation is typically associated with creating new content. As a result, it does not tend to have an method of undoing the transformation or a reversible animation.
  
### Large Screens
1. A floating action button can attach to an extended app bar.
2. A floating action button can be attached to a toolbar or structural element within a sheet (as long as it’s not blocking other elements).
3. A floating action button can be attached to the edge of a sheet.
4. Don’t have more than one floating action button per screen.
5. Don’t associate floating action buttons with every element on a screen.
