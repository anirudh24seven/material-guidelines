## Bottom sheets
1. A bottom sheet is a sheet of material that slides up from the bottom edge of the screen and presents a set of clear and simple actions.
2. Bottom sheets are primarily a mobile component.

### Usage
1. Bottom sheets are best suited to displaying three or more actions that do not require a description. If there are fewer than three actions, or a detailed description is required, consider using a menu or dialog instead.
2. You can use bottom sheets to show actions related to other apps, or to allow entry points to other apps (via the app icon).
3. Bottom sheets can be list-style or grid-style. Grid layouts are easier to scan.

### Content
1. In a list-style bottom sheet, each action should have a text description and a left-aligned icon. Use subheaders or titles to give context to the choices.
2. When necessary, use separators to group actions logically.
3. A scrollable grid-style bottom sheet can contain icons for share actions.

### Behavior
1. When a bottom sheet is displayed, it animates upwards from the bottom edge of the screen. The rest of the screen dims, giving focus to the bottom sheet. Tapping outside of the bottom sheet, or swiping the bottom sheet downward, dismisses it.
2. If the bottom sheet contains more actions than can fit, the bottom sheet is scrollable. Scrolling may eventually allow the bottom sheet to expand to cover the entire screen. Add a dismiss button to the header, on the left side of the title, so users can easily dismiss an expanded bottom sheet.

### Specs

The following specs are provided for mobile apps.

Font and color:

1. Text: Roboto Regular 16sp,  #000 87%
2. Title (optional): Roboto Regular 16sp, #000 54%
3. Default bottom sheet background fill: #FFF
4. Overlay shield fill: #000 20%
