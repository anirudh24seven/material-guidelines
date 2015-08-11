## Menus

Menus allow users to take an action by selecting from a list of choices revealed upon opening a temporary, new sheet of material.

### Usage
1. A menu is a temporary piece of material emitted from a button, an action, a pointer, or another control that contains at least two menu items.
2. Each menu item is a discrete option or action that can affect the app, the view, or selected elements within a view.
3. Menus should not be used as a primary method for navigation within an app.
4. The label of an emitting button or control concisely and accurately reflects the menu items contained within the menu. Menu bars typically use single words as labels, like “file,” “format,” “edit,” and “view,” while other contexts may have more verbose labels.
5. Menus display a consistent set of menu items, each of which may be enabled or disabled based on the current state of the application.
6. Contextual menus dynamically change their available and enabled menu items based on the current state of the application.
7. Generally, remove menu items that are irrelevant to the current context, and disable menu items which are relevant but need certain conditions to be met (for example, Copy becomes enabled when text is selected).
8. Certain application states may result in a contextual menu containing only a single menu item. For example, when highlighting text on a web page, Android reveals only Copy, since users cannot cut or paste text.
9. If the height of a menu prevents all menu items from being displayed, the menu can scroll internally. One example is when viewing a menu on a phone in landscape orientation.
10. Desktop: a menu can also cascade. Reposition menus vertically and horizontally based on their proximity to screen edges.
11. Desktop: These animations show scrolling and cascading menus in action.
12. Note: Implementations of this component may vary by platform. By using standard platform implementations, you will receive any related future improvements.

### Menu items
1. Each menu item is limited to a single line of text that describes the action it will perform when selected.
2. The text is generally a single word or short phrase, but it can include icons and helper text, like keyboard shortcuts, as well as controls like checkmarks to indicate multiple selected items or states. See also List controls.
3. Menus with static content should have the most frequently used menu items placed at the top of the menu.
4. Menus with dynamic content may have other behavior, such as placing previously used fonts at the top of the menu. The order can change based on user actions.
5. Menu items can reveal nested submenus. Try to limit nesting to one level deep, as it can be difficult to navigate multiple nested submenus.
6. Displaying actions as disabled, rather than removing them, lets the user know they exist under the right conditions.
7. For example, Redo is disabled when there is nothing to redo. Cut and Copy are disabled until content is selected.

### Behavior
1. Menus appear above all other in-app UI elements.
2. Dismiss a menu by tapping outside of the menu, or by tapping the emitting button (if visible).
3. Generally, selecting a menu item will also dismiss the menu. An exception is when a menu allows for multiple items to be chosen, for example, by using checkmarks.
4. Menus are positioned over their emitting elements such that the currently selected menu item appears on top of the emitting element.
5. Do not display a duplicate of the selected menu item.
6. Positioning the menu below the emitting element separates it from its context.

### Simple Menus
1. When close to a screen edge, simple menus reposition their vertical alignment so that all menu items are completely visible.
2. Simple menus are used in list views on tablet and mobile devices to display the options for a specific list item.
3. Disambiguation: In contrast to simple menus, simple dialogs can present additional detail related to the options available for a list item or provide navigational or orthogonal actions related to the primary task. Although they can display the same content, simple menus are preferred over simple dialogs because simple menus are less disruptive to the user’s current context.
4. Use simple menus in lists to display the options for a specific list item.
5. Choosing an option immediately commits the option and closes the menu.
6. Touching outside of the menu, or pressing the system Back button, cancels the action and closes the menu.
7. When opened, simple menus attempt to vertically align the currently selected menu item with the list item. The currently selected menu item is highlighted.
8. Do not arbitrarily position the first menu item over the list item.
9. When close to a screen edge, simple menus reposition their vertical alignment so that all menu items are completely visible.
10. Simple menus appear over their emitting element, not below.
11. Menu width varies depending on string length, and on mobile is defined as a multiple of a 56dp unit.
12. Simple menus always maintain a 16dp margin (phone) or 24dp margin (tablet) to the left and right edges of the screen.
13. If text in a simple menu wraps to a second line, use a simple dialog instead. Simple dialogs can have rows with varying heights.
14. Menus show a persistent scroll bar when content is scrollable.
15. The maximum height of a simple menu should be one or more rows less than the view height. This ensures a tappable area outside of the simple menu with which to dismiss the menu.
16. Don’t duplicate the selected menu item.
17. Simple menus are always left-aligned with the start of the list item text and do not reposition horizontally based on touch location.

### Specs

Specs are provided for various sizes and types of menus and for different platforms. Add 8dp padding at the top and bottom of a menu.

1. Mobile
2. Various widths
3. Cascading menu
4. Cascading redlines
