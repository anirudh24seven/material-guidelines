## Errors
1. Errors occur when an app fails to complete what is expected, such as:
  1. The app does not understand user input
  2. The system or app fails
  3. A user intends to run incompatible operations concurrently
2. Minimize errors by designing apps that make it easy for users to input information flexibly. Apps should accept common data formats that use affordances to improve user understanding.
3. How to address errors:
  1. Clearly communicate what is happening
  2. Describe how a user can resolve it
  3. Preserve as much user-entered input as possible
  
### User input errors
1. Help users fix input errors as soon as they are detected. Disable the submission of a form if errors are detected, and if detected only after form submission, clearly explain the error and how to fix it.
2. Text field input  
  1. Helper text may be included before, during, or after a user interacts with each field on a form.
  2. Show error text only after user interaction with a field. If the user inputs incorrect data, helper text may transform into error text.
  3. Minimize form text to the essentials. Not every text field needs helper and/or error text.
  4. Specification:
    1. Place 16dp of vertical space between text fields and the below error text.
  5. Fonts for light backgrounds
    1. Errors: Roboto Regular 12sp #DD2C00
    2. Hint and helper text: #000000 with 38% opacity
  6. Fonts for dark backgrounds
    1. Errors: Roboto Regular 12sp
    2. Hint and helper text: #FFFFFF with 30% opacity
  7. Helper and error text
  8. Error with floating text label
3. Text field input - Over/under character or word count
  1. A character counter may be displayed before, during, and after user interaction with a field. Consider not displaying the counter until the user approaches the character limit.
    1. Counter font is Roboto Regular 12sp
    2. Counter fields have 16dp of additional bottom padding
  2. Single-line with character counter
  3. Multi-line with character counter
4. Incompatible values
  1. Show errors for incompatible values during or after a user interacts with a text field.
  2. If two or more fields have incompatible inputs:
    1. In the text field, indicate a fix is needed. Add an error message below.
    2. Display a message at the top of the form, or screen, summarizing the fixes needed and any additional explanation.
5. Errors detected upon form submission
  1. Reload the form with consolidated error messages and scroll position at the top. Error messages for individual fields may be resolved as the user works through the form.
6. Incomplete form
  1. Empty form fields should be indicated by both the text field and error message below.
  2. Display incomplete form errors to indicate a user has skipped a field after they have advanced through a form. If unable to detect user progress through the form, display an error after the user has attempted to submit the form.
7. Multiple errors before form submission
  1. Individually label error messages as the user works through the form.
8. Single-line list error

### App errors
1. App errors occur independent of user input.
2. General app error
  1. When an error occurs, an app should display loading indicators until the error message appears.
  2. Features not available may be represented in the UI. Not every error requires a new component to pop up.
  3. If possible, give your user an action that will help them address the error.
3. General app error
  1. When an error occurs, an app should display loading indicators until the error message appears.
  2. Features not available may be represented in the UI. Not every error requires a new component to pop up.
  3. If possible, give your user an action that will help them address the error.
4. Connectivity
  1. When connectivity is down, the user should be able to interact with as much of the rest of the app as possible.
  2. If appropriate, present a link to help a user accomplish their task. Only offer links that you can actually support. For example, don't offer an option like "Try again" in cases where you can detect that the operation will fail.

### Incompatible state errors
1. Incompatible state errors occur when users attempt to run operations that conflict, such as making a call while in airplane mode or taking a screenshot from a restricted work account. Help prevent users from putting themselves into these situations by clearly communicating the states they are selecting and the implications for the rest of their experience. When these errors are triggered, do not imply that they are the user’s fault.
2. General incompatibility
  1. Clarify the reason for and origination of the error.  
  2. For example, screenshots and premium features are not allowed while in a restricted mode.
3. Offline by choice
  1. Display an unobtrusive, persistent indicator when users are offline but try to do tasks that require being online.
  2. Examples:
    1. Placing a call while in airplane mode
    2. Music availability while offline
4. Permission requested
  1. If your app requires user permission before proceeding with an action, include the permission request in the app flow instead of treating it as an error.
  2. If permissions are necessary before the first run of an app, consider including them into your app’s first-run experience.
  3. Examples:
    1. An app’s permissions have changed.
    2. In-app purchases have been disabled.
