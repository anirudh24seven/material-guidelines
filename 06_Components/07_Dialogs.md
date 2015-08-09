## Dialogs
1. Dialogs inform users about critical information, require users to make decisions, or encapsulate multiple tasks within a discrete process. Use dialogs sparingly because they are interruptive in nature. Their sudden appearance forces users to stop their current task and refocus on the dialog content. Not every choice, setting, or detail warrants interruption and prominence.
2. Alternatives to dialogs include menus or inline expansion within the current content area. Both approaches present non-interruptive options while maintaining the current context.

### Content
1. Dialog content can vary widely, but typically consists of text and/or UI control elements focused on a specific task or process. Examples include confirming item deletion or choosing a setting.
2. To disclose additional content, use inline expansion within the content area of dialogs, such as advanced options.
3. Avoid dialogs that:
  1. Open additional dialogs from within a dialog.
  2. Contain scrolling content, particularly alerts. Instead, consider alternate containers or layouts that are optimized for reading or interacting with significant amounts of content.
4. Exceptions include:
  1. Full-screen dialogs may open additional dialogs, such as pickers, because their design accommodates additional layers of material without significantly increasing the app’s perceived z-depth or visual noise.
5. Use and limitations: 
  1. Dialogs are a sub-type of modal windows, and the examples covered here are for standard material system dialogs.
  2. Other modal window constructions aren’t covered here because they have too much variation. For example, they can include elements such as branded buttons for purchasing flows, non-standard UI form elements, illustrations, or unique layouts.
  
### Behavior
Dismissing dialogs

1. Dialogs are separate from the underlying parent material and do not scroll with the parent material.
2. Some dialog content requires scrolling, such as lists of ringtones. If the content is a scrollable list of options, the dialog title remains pinned to the top. This behavior means that a currently selected item in a scrollable list can be visible simultaneously with the title, regardless of the item’s position in the list. Otherwise, the title scrolls off with the content. Actions always remain in place when content scrolls.
3. Dialogs should never be obscured by other elements and should never appear only partially on screen. Dialogs always retain focus until they have been affirmed or dismissed or a required action has been taken, such as choosing a setting.
4. Dialogs can be dismissed by touching/clicking outside of the dialog or by using the system back button (Android). Dialog behavior can be overridden so that users must explicitly choose one of the actions.
  
### Alerts
1. Alerts inform the user about a situation or action that requires their confirmation or acknowledgement before proceeding. They differ slightly in appearance based upon the severity and impact of the message conveyed.
2. Alerts are interruptive, urgent, and prevent users from proceeding until they make a decision.
3. Disambiguation from Snackbars: In contrast to Alerts, Snackbars present optional but important information or actions and usually appear after an action. For example, use an alert to confirm discarding a draft. Use a snackbar to present an undo action, because the action is optional and the user can continue with their primary task without taking action.
4. Alerts without title bars
  1. Most alerts don't need titles. Usually the decision doesn't have a severe impact and can be summed up succinctly in a sentence or two. The content area should either ask a question (such as "Delete this conversation?") or make a clear statement whose relationship to the action buttons is obvious.
5. Alerts with title bars
  1. Use alerts with title bars sparingly. They are appropriate only for high-risk situations, such as potential loss of data or connectivity, or extra charges.
  2. If a title is required:
    1. Use a clear question or statement with an explanation in the content area. For example, "Erase USB storage?"
    2. Avoid apologies and ambiguous statements or questions. For example, don’t use “Warning!” or “Are you sure?”
  3. A user should be able to skip the content completely and still have a clear idea of what choices are available based on the title and the text of the action buttons.
  
### Simple menus
1. Simple menus are used in list views on tablet and mobile devices to display the options for a specific list item. Simple menus immediately commit choices upon selection. See Components > Menus > Simple Menus for more details.
2. Disambiguation: In contrast to simple menus, simple dialogs can present additional detail related to the options available for a list item or provide navigational or orthogonal actions related to the primary task. Although they can display the same content, simple menus are preferred over simple dialogs because simple menus are less disruptive to the user’s current context.

### Simple dialogs
1. Simple dialogs can present additional details about a list item or provide actions related to the primary task. For example, simple dialogs can display avatars, icons, or clarifying subtext, or they can enable users to perform an orthogonal action such as adding an account that’s not currently listed as an option.
2. Touch mechanics:
  1. Choosing an option immediately commits the option and closes the menu.
  2. Touching outside of the dialog, or pressing Back, cancels the action and closes the dialog.
3. Simple dialogs are more interruptive than simple menus and should be used sparingly.
4. Simple dialogs do not have explicit buttons that accept or cancel the operation.
5. Specifications:
  1. A simple dialog appears centered vertically and horizontally in the screen.
  2. The distance between the edges of the screen and the edges of the dialog is minimum 40dp on the left and right, and minimum 24dp on the top and bottom.
  3. The distance between the edge of the dialog and content is 24dp.
6. Row heights can vary in simple dialogs.
7. If any text in a simple menu wraps to another line, use a simple dialog instead.

### Confirmation dialogs
1. Confirmation dialogs require users to explicitly confirm their choice before the option is committed. For example, users can listen to multiple ringtones but make a final selection only upon touching “OK.”
2. Touching “Cancel” in a confirmation dialog, or pressing Back, cancels the action, discards any changes, and closes the dialog.
3. Confirmation dialogs can use layouts other than lists, for example a date picker, but they are still focused on specifying a single value (picking the date, but not picking the time and date).
4. Confirmation dialogs provide both an explicit confirmation button and explicit cancel button. The explicit cancel button clarifies that leaving the confirmation dialog will discard changes, for example, by touching cancel or pressing Back.
5. Confirmation dialogs should avoid launching additional simple dialogs or simple menus. The additional layers of material can increase the app’s perceived z-depth, and add unnecessary visual complexity.
6. If additional simple dialogs or simple menus are needed to complete the task or process, consider using a full-screen dialog instead of a confirmation dialog.

### Full-screen dialogs
1. Mobile only: Due to limited real estate on mobile devices, dialog content appearing in other form factors (tablet, desktop, etc.) may be more appropriate on mobile using a full-screen dialog.
2. Usage
  1. Full-screen dialogs group complex tasks that require explicit action, such as save or create, before changes are committed or discarded, as in a calendar entry.
  2. Full-screen dialogs enable complex layouts, minimize the appearance of stacked sheets of material (dialogs above dialogs) and increase the app’s perceived z-depth. They enable individual tasks to launch simple menus or simple dialogs as part of the complex operation.
  3. Consider using a full-screen dialog when the content or process meets any of the following criteria:
    1. The dialog includes components like pickers or form fields requiring an input method editor (IME), such as a keyboard.
    2. When changes are not saved in real time
    3. When there is no draft capability in the app
    4. When performing batch operations or queuing changes prior to submitting them
  4. No modifications and selections made in the full-screen dialog are saved until “Save” is touched. Touching the “X” will discard all changes and exit the dialog.
3. Actions
  1. In full-screen dialogs, the confirmation and dismissive actions are at the top of the screen.
4. Confirmation
  1. The confirmation action is at the top right of the screen and uses descriptive and accurate verbs, such as “save,” “send,” “add,” “share,” “update,” or “create.”
  2. Don’t use vague actions such as “done,” “ok” or “close” for the confirmation action. They are too similar in meaning to the X and non-specific in their result.
  3. The confirmation action is disabled until all mandatory criteria in the dialog are met.
5. Discard
  1. The discard action, an “X” at the top left of the screen, closes the full-screen dialog and discards any changes. The Back button is equivalent to the discard action.
  2. If the user has made any changes, they are prompted to confirm the discard action. If no changes have been made, touching the “X” or “Back” immediately closes the dialog and no discard confirmation is required.
6. Navigation
  1. The “X” used in a full-screen dialog differs from an up arrow, which indicates the view’s state is constantly being saved or when apps enable draft or autosaving. For example, an up arrow is used in Settings because all changes are committed immediately. In these cases, the Back button navigation and action match the up arrow functionality, and there are no explicit confirmation or cancel actions.
7. Titles
  1. Full-screen dialog titles don’t use dynamic type.
  2. Titles should be succinct.
  3. Full-screen dialog titles can wrap to a second line if necessary, and then should be truncated.
  4. If the full-screen dialog uses titles of variable length or anticipates long titles (for example, because certain words are longer in different languages), place title text in the content area of the dialog instead of the app bar.

### Specs
1. Dialogs contain an optional title, content, and actions.
2. The optional title briefly describes the type of choice being made. Titles should always be displayed in their entirety and should be used only when necessary. Titles can be used to clarify the decision being made. For example, a title may indicate what part of a process the dialog relates to or identify what will be affected by the decision, such as a setting.
3. Dialog content can vary widely, but typically consists of text and/or UI control elements and is focused on a specific task or process, such as confirming item deletion or choosing a setting.
4. When needed, actions acknowledge, affirm, or dismiss the particular choice or process presented by the dialog content.
5. A note on accessibility
  1. To ensure usability for people with disabilities, make sure that your buttons have a minimum height of 36dp, but that the touchable target has a minimum height of 48dp.
  2. The default color of all dialog action text is the system color. The system color can be overridden to use the application’s theme accent color. Make sure that the combination of accent color and action text doesn’t impart unintended meaning. For example, red text implying warning or danger for a non-destructive confirmation action.
  3. Always make sure the action text color uses a sufficient contrast ratio to meet accessibility guidelines. Change the default text color as needed to create a sufficient contrast ratio.
6. Actions
  1. Dialogs present a focused and limited set of actions, which are generally affirmative or dismissive.
  2. Affirmative actions are placed on the right side and continue the process. Affirmative actions may be destructive, like “Delete” or “Remove”.
  3. Dismissive actions are placed directly to the left of affirmative actions and return the user to the originating screen or step in the process.
  4. Dismissive and affirmative action text can be “Cancel”/”OK” or can be more specific active verbs or verb phrases that indicate the outcome of the decision.
7. Dialog actions should make decisions as easy as possible by presenting a clear, unambiguous choice that directly relates to the dialog’s title and content.
  1. Clearly state a potential result in the dialog title.
  2. The dialog content should directly relate to the title or choices.
  3. Present clear choices.
8. For languages without capitalization (for example, Chinese, Japanese, or Korean), the consistent placement and spacing of actions in the bottom-right corner of the dialog, along with text color, help distinguish dialog actions from regular dialog text.
9. In particular, because a dismissive action is never disabled, and because the positioning of dialog actions places the dismissive action before the affirmative action in reading order, a disabled affirmative action is prevented from appearing like regular dialog text.
10. In situations where users are required to acknowledge the dialog’s content prior to proceeding, an alert may contain only one action. However, this type of alert should be used sparingly as it is interruptive and does not provide users with a decision to make or choose an action. Consider other methods of communicating the information to users, such as in-line with a view’s content.
11. Dialogs generally should not include more than two actions. A third action such as “Learn more” that navigates away from the dialog or app leaves the current task and decision in an indeterminate state.
12. Avoid using a “Learn more” action in a dialog to access help documentation. If a little more detail or explanation is needed for the dialog contents, use in-line expansion within the dialog. If more extensive information or explanation is needed for the dialog content, provide that information prior to entering the dialog.
13. Content guidelines
  1. Padding around content area: 24dp
  2. Padding between title and body text: 20dp
  3. Padding around buttons: 8dp
  4. Button height: 36dp
  5. Action area height: 52dp
  6. Dialog elevation: 24dp
14. Button width and padding
  1. Button height: 36dp
  2. Minimum button width: 64dp
  3. Internal button padding: 8dp
  4. Padding between buttons: 8dp
  5. Button area height: 52dp
  6. Left button padding: 24dp
  7. Right button padding: 8dp
  8. Padding between buttons: 8dp
15. Side-by-side buttons
  1. Side-by-side buttons are recommended when the text of each label does not exceed the maximum button width, such as the commonly used OK/Cancel buttons.
  2. Use the following formula to calculate maximum button width for a given dialog:
    1. The maximum width for buttons in a dialog = (Dialog width - 8dp - 8dp - 8dp)/2
  3. For example:
    1. The maximum width for buttons in a 280dp wide dialog = (280dp - 8dp - 8dp - 8dp)/2 = 128dp
16. Stacked full-width buttons
  1. When text labels exceed the maximum button width, use stacked buttons to accommodate the text. Affirmative actions are stacked above dismissive actions.
17. Simple dialog keylines
  1. Vertical keyline at 24dp from the left and right edges. Content associated with an icon or avatar aligns 80dp from the left edge.  
18. Full-screen dialog titles
  1. Full-screen dialog titles can wrap to a second line if necessary, and then should be truncated. Titles should be succinct, but in some situations, such as when words are longer in different languages, titles may need to wrap.
    1. App bar height with a single line of text: 56dp
    2. App bar height with two lines of text: 80dp
    3. Title text keyline: 72dp
    4. Title text: 20sp
    5. Title text top and bottom padding: 20dp
    6. Dismissive action padding from left edge: 16dp
    7. Affirmative action text: 14sp
    8. Affirmative action text padding on the left and right: 16dp
    







  
  
  
