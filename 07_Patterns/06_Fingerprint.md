## Fingerprint
1. Android only
2. Fingerprint detection can be used to unlock a device, sign in to apps, and authenticate purchases with Google Play and some third-party apps.
3. Fingerprint is not as secure as a strong PIN or password.

### Enrollment
1. Before invoking Fingerprint in your app, you must get consent from the user that they want to use Fingerprint as an alternate way of authenticating themselves.
2. Possible times to invite users to try Fingerprint include:
  1. Upon opening the app
  2. During your app’s purchase flow
  3. In your app settings
  4. After enrollment

### Authentication
1. Your app’s users can set up the option to log in or authenticate purchases using Fingerprint.
2. When a user action needs to be authenticated, display the Fingerprint authentication dialog in place of your login screen.
3. Title
  1. Use the title to describe the action being performed, such as “Sign in.” The title should not be used to introduce Fingerprint.
4. Secondary text
  1. Use the phase “Confirm fingerprint.” This wording maintains consistency with Android Settings.
  2. You may combine the above text with the associated user action, such as “Confirm fingerprint to complete purchase.”

### Behavior
1. Default state
  1. Ask the user to put their finger on the sensor.
2.  Success state
  1. Once the fingerprint is recognized, change the dialog to a success message and the image to the fingerprint icon with the check mark.
  2. Specification:
    1. Use your app’s primary color for the success text and icon, or Teal 500 (#009688)
  3. Success states should avoid:
    1. Displaying two success states simultaneously
    2. Extensive transitions between default and success states
3. Failure state
  1. Upon failure, provide a clear indication that the user’s fingerprint was not recognized and that they should try again, using the error icon either with or without a status message.
  2. Specification:
    1. Use your app’s color assigned to failure states, or Deep Orange 600 (#F4511E)
  3. Failure states should avoid:
    1. Extensive transitions between default and failure states
4. Exiting
  1. Provide alternative ways to exit the dialog. At minimum, provide an affordance to close the Fingerprint dialog, such as a “Cancel” button.
5. Authentication alternatives
  1. Fingerprint should not be the only way to authenticate. Provide alternative authentication methods, such as:
    1. User’s account password
    2. App PIN
    3. Device credentials

### Fingerprint icon
1. Usage and size
  1. The Fingerprint icon should be displayed at the standard system icon size, 24dp, within a 40dp circle.
2. Default icon
  1. Users will be asked to look for this icon for places where they can use Fingerprint.
  2. Specifications:
    1. Circular background color: #607D8B
    2. Works on white backgrounds
3. Tinted icon
  1. The circle surrounding the icon can be customized with a color that provides appropriate contrast against the lines of the Fingerprint icon.
4. UIs with light backgrounds
  1. Use the Fingerprint icon with a dark circle background.
  2. Specifications:
    1. Color: #FFFFFF
    2. Opacity: 100%
5. UIs with dark backgrounds
  1. Use the Fingerprint icon with a light circle background.
  2. Specifications:
    1. Color: #000000
    2. Opacity: 54%
6. Icon with no circular background
  1. Apps requiring a more versatile Fingerprint icon may eliminate the circular background.

### Reauthentication
1. Reauthentication applies when users need to confirm their identity before continuing.
2. Reauthentication uses:
  1. To prevent unauthorized viewing of sensitive information
  2. To guard against unauthorized purchases
  3. When cryptographic keys expire and users are asked to reconfirm their identity
3. Alternatively, if a user forgets about Fingerprint authentication, you can ask users to use their backup password and remind them of the Fingerprint option next time.
  
