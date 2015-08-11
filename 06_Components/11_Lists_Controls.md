## Lists: Controls

List controls are icons that appear to the left or right of the list text. They indicate the state of a list item, information about a list item, or serve as an action related to the list item. Leave-behinds are list controls, which are revealed only upon swipe.

### Usage
1. List controls fall under four categories:
  1. State
  2. Primary action (including text strings)
  3. Secondary action
  4. Secondary info
2. Distinguishing elements of list tiles need to be on the left for Left-to-Right interfaces, and vice versa. States and primary actions are placed on the left side of a list tile. Text within a list item should be considered part of the primary action target.
3. Don’t place two icons or actions next to one another, such as a checkbox next to an avatar.
4. If the primary action of the list item is navigational, don’t use an icon. The list item itself and its context should be sufficient to communicate the destination.
5. Secondary actions and info should be placed on the right side of the title. Secondary actions are always a separate target from the primary action, as users increasingly expect every icon to trigger an action.

### Types of list controls
1. Checkbox - A checkbox can either be a primary action or a secondary action.
  1. Type: primary action/state
    1. Desktop checkboxes should appear only on hover and focus. 
  2. Type: secondary action
    1. Separate target
    2. When controlling a family of variables, consider using switches instead.
2. Switch
  1. Type: secondary action
  2. Separate target
3. Reorder
  1. Type: secondary action
  2. Usually a separate target, depending on which mode list it is in.
  3. Allows dragging of the list item to other locations within the list. It usually appears in list editing mode.
4. Expand/collapse
  1. Type: secondary action
  2. Separate target
  3. Expands and collapses a list view vertically to show and hide details of existing list items.
5. Leave-behinds
  1. Type: Other
  2. A leave-behind is an informative hint as to what swiping a list item away will do to that item. The leave-behind can transform into an action.
  3. Swiping on a list item from either direction will reveal an icon indicating the action. After swiping, a follow-up action can appear as a text button within the space of the list item.
  
### Types of menu controls

A menu is a special type of list. In menus, use controls that are appropriate for dropdown menus, overflow menus, and so on. Don’t use these controls in regular lists. Use the regular list controls instead.

1. Check
  1. Type: state
  2. Not a separate target.
  3. Menus only. Indicates that the list item has been selected. The selection is done through a different control.
2. Inline information
  1. Type: secondary info
  2. Not a separate target.
  3. Menus only. Inline information is a small snippet of text related to the line title that can provide information or a tip, like a keyboard shortcut. It cannot be truncated.
