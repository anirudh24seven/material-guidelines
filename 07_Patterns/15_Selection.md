## Selection
1. Selection involves both the gestures and visual cues that allow users to make choices.
2. The global gesture to select data is a long-press, a touch or mousedown that’s held in the same position for a moment. A two-finger touch may also trigger selection on touch devices.
3. Checkboxes, or custom analogs, should not be used for selection on mobile. They should only be used for contexts in which checking an item indicates completion, such as task lists or checklists, rather than selection.
4. Checkboxes may be used on desktop with the following guidelines:
  1. Avoid persistently displaying checkboxes as part of each item.
  2. When hovering on an item, display a single checkbox for that item.
  3. After an item has been selected, display checkboxes for all remaining items in that set.

### Item selection
1. Support for multi-selection is strongly recommended for list and grid containers. This does not apply to actions available for a single selection (like a list of phone numbers, where calling is the only action), or if the context requires single-item manipulation (like moving icons on Android’s home screen).
2. Gestures:
  1. When initiating selection, both long-press and two-finger touch may be extended using a drag gesture to select multiple items. Items between the beginning and end points of the drag will be included in the selection.
  2. On desktop, a drag originating outside the bounds of all items may initiate multi-selection (for example, beginning a drag in the left margin of a list, and extending down and to the right to select list items).
3. Once an initial selection is made, it can be altered through user actions:
  1. Touch a selected item to deselect it. Touch an unselected item to select it.
  2. Shift+touch/click on an item to select all items between two selected points.
  
### Text selection
1. Text selection is indicated by highlighting the bounds of the selected text.
2. On mobile, a selection handle is added to both the beginning and end of the selection. Actions related to the text appear in a dropdown menu positioned immediately above, but not overlapping, the selection.
3. Text selection must occur in one contiguous block. However, the bounds of the selection may be altered through user action:
  1. Dragging the initial selection to expand the selection
  2. Dragging either of the selection handles to expand or reduce the selection
  3. Touching (or clicking) repeatedly within the selection to expand it (single word > paragraph > all)
  4. Keyboard shortcuts
    1. Shift+Left/Right Arrow: Character-by-character selection
    2. Shift+Up/Down Arrow: Line-by-line selection
    3. Ctrl/Command+A: Select all
  5. Text selection handles
  6. Text selection - light theme
  7. Text selection - dark theme
4. Text selection toolbar
  1. The floating toolbar appears above the selection area with primary actions of Cut, Copy, Paste, and More. When the user selects the More icon, the toolbar collapses and transforms into a secondary menu to reveal additional actions.
  2. The font for the floating toolbar text is Roboto Medium 14sp, all caps.
