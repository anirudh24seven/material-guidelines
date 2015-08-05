## Buttons
A button clearly communicates what action will occur when the user touches it. It consists of text, an image, or both, designed in accordance with your app’s color theme.

### Usage
1. There are three standard types of buttons:
  1. Floating action button: A circular material button that lifts and displays an ink reaction on press.
  2. Raised button: A typically rectangular material button that lifts and displays ink reactions on press.
  3. Flat button: A button made of ink that displays ink reactions on press but does not lift.
  
2. Choosing button style

  Choosing a button style depends on the primacy of the button, the number of containers on screen, and the screen layout.
  1. Function: Is it important and ubiquitous enough to be a floating action button?
  2. Dimension: Choose raised or flat depending on the container it will be in and how many z-space layers you have on screen. There should not be many layers of objects on the screen.
  3. Layout: Use primarily one type of button per container. Only mix button types when you have a good reason to, such as emphasizing an important function.
  
3. Buttons in dialogs

  Use flat buttons on dialogs to prevent too many layers of dimension.

  1. Text content: 16dp padding from dialog edge
  2. Dialog button container: 48dp tall, 16dp below text content, 8dp from dialog bottom edge
  3. Dialog buttons: 36dp tall, vertically aligned in middle of button container, 16dp from container right edge (for LTR scripts)
  
4. Buttons inline
  1. Choose raised or flat buttons depending on your layout. Add padding around flat buttons so the user can easily find them.
  
5. Persistent footer buttons
  1. If your app requires actions to be persistent and readily available to the user, consider using the floating action button.
  2. Alternatively, consider persistent footer buttons, which are also easily accessible.
  3. Never use raised buttons within persistent button areas.
  4. With the addition of a divider, a persistent footer button can also be used for scrollable dialogs.
  
### Flat & raised buttons
1. Raised buttons
  1. Raised buttons add dimension to mostly flat layouts. They emphasize functions on busy or wide spaces.
2. Flat buttons
  1. Use flat buttons for toolbars and dialogs to avoid excessive layering.
3. Flat and raised button states
  1. Raised buttons behave like a piece of material resting on another sheet—they lift and fill with color on press.
  2. Flat buttons are printed on material. They do not lift but fill with color on press.
  3. Button text should be all caps in languages that have capitalization. For languages that don’t have capitals, consider using colored text for flat buttons to make them stand out from normal text.
4. Accessibility
  1. To ensure usability for people with disabilities, make sure that buttons have a height of 36dp and touchable targets have a minimum height of 48dp.
5. Buttons in motion

### Other buttons
1. Icon toggles
  1. Icons are appropriate for app bars, toolbars, action buttons or toggles.
  2. Icon toggles can display bounded or unbounded ink ripples beyond their touch target bounds. For more information, see Surface Reaction.
2. Mobile dropdown buttons
  1. Dropdown button
    1. A dropdown button selects between multiple selections. The button displays the current state and a down arrow. Available states may be shown as a list of strings, a palette, or icons, for example.
    2. When a user interacts with the button, a menu covers the button and displays the possible states. Pressing a state dismisses the menu and updates the button to display this new state.
    3. Scrolling within the dropdown behaves the same way a menu scrolls.
  2. Generic overflow dropdown button
    1. This button is a dropdown button that does not have a displayed state but has an arrow or a generic menu button. When the button is pressed, the menu flies out. Pressing an option on the menu generally navigates to further settings for that option.
  3. Segmented dropdown button
    1. A segmented dropdown has two sections: the current state and the dropdown arrow icon. Pressing the current state will cause that state’s action to fire within the screen. Pressing the dropdown arrow will display all the state options. Selecting one will change the displayed state.
  4. Editable segmented dropdown button
    1. This button has a segmented dropdown, where the displayed state is text editable, such as a font size picker. Pressing the current state causes both that state’s action to fire and makes the displayed state editable. Pressing the arrow displays all the state options.
3. Desktop dropdowns
  1. Desktop app bar specs
