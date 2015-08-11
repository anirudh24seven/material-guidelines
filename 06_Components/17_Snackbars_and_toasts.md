## Snackbars & toasts
1. Snackbars provide lightweight feedback about an operation by showing a brief message at the bottom of the screen. Snackbars can contain an action.
2. Android also provides a toast, primarily used for system messaging. Toasts are similar to snackbars but do not contain actions and cannot be swiped off screen.

### Usage
1. Show only one snackbar on screen at a time.
2. Placement
  1. Snackbars appear above most elements on screen, and they are equal in elevation to the floating action button. However, they are lower in elevation than dialogs, bottom sheets, and navigation drawers.
3. Behavior
  1. Upon entrance, snackbars animate upwards from the bottom edge of the screen. When they appear, they do not block input.
  2. They exit by being swiped off-screen or automatically disappear after a timeout or user interaction elsewhere (such as summoning a new surface or activity).
4. Very short text strings
  1. Snackbars should contain a single line of text directly related to the operation performed. They may contain a text action. They cannot contain icons.
5. Transient
  1. Snackbars automatically time out from the screen. For usability reasons, snackbars should not contain the only way to access a core use case. They should not be persistent or be stacked, as they are above other elements on screen.
  2. On Android, when an unrelated dialog or popup occurs while the snackbar is up, the snackbar timeout will reset upon the window focus being regained. This is to ensure that the user will be able to read the snackbar for the full intended duration.
6. 0-1 actions, not dismiss or cancel
  1. If an action is present, comply with dialog spacing and affordance rules. For two or more actions, use a dialog, not a snackbar, even when one of the actions is a dismiss action. If the action described in the snackbar is important enough to block the use of the screen, it should be a dialog.
7. Don’t block the floating action button
  1. Move your floating action button vertically to accommodate the snackbar height.
8. Consecutive snackbars
  1. There is only ever one snackbar displayed. When a second snackbar is triggered while the first is displayed, the first should start the contraction motion downwards before the second one animates upwards.

### Specs
1. Mobile
  1. Single-line snackbar height: 48dp
  2. Multi-line snackbar height: 80dp
  3. Text: Roboto Regular 14sp
  4. Action button: Roboto Medium 14sp, all-caps text
  5. Default background fill: #323232 100%
2. Tablet/desktop
  1. Single-line snackbar height: 48dp tall
  2. Minimum width: 288dp
  3. Maximum width:  568dp
  4. 2dp rounded corner
  5. Text: Roboto Regular 14sp
  6. Action button: Roboto Medium 14sp, all-caps text
  7. Default background fill: #323232 100%  
  
