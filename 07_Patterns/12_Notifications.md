## Notifications
1. Android only
2. Notifications inform your app’s users about relevant and timely events in your app. You can create notifications to draw attention to messages from friends, alert a commuter to traffic slowdowns, show the progress of a new app being installed, and more. They are synced to all of a user's devices.

### Usage
1. Minimize interruption
  1. Notifications inform users about events in your app while the user is focused elsewhere. As they can be interruptive, use notifications judiciously.
  2. Notifications should not be used for:
    1. Information that is currently on screen (such as an active chat conversation)
    2. Technical operations that don’t require user involvement (such as syncing)
    3. Transient error states that can resolve without user action
2. Make notifications optional
  1. Users should always be in control of notifications. Allow users to disable or change notifications in your app’s settings.

### Guidelines
1. Prioritize social interactions
  1. Use notifications for events that involve other people.
2. Be timely
  1. Notify the user about time-sensitive information directed specifically at them.
3. Personalize notifications
  1. For notifications sent by another person, include that person's image.
  2. Your app’s icon is shown paired with the personalized image.
4. Navigate to the right place
  1. When the user touches a notification, enable the user to take immediate action on it. This may open a detail view, such as a message, or a summary view for multiple notifications.
5. Prioritize notifications
  1. Android allows you to set priority flags to influence where your notification appears relative to others.
6. Summarize notifications
  1. If multiple notifications of the same type are available, combine them into a single summary notification. A summary shows how many notifications of a particular kind are pending.
  2. You can provide more detail about notifications in a summary with the expanded digest layout.
7. Use distinct icons
  1. Pending notification icons should be recognizable in the system bar.
  2. Notification icons should:
    1. Be distinct from existing Android notification icons
    2. Follow guidelines for system icon styling
    3. Be visually simple
    4. Be opaque white, using only the alpha channel
    5. Have a transparent background
  3. They may have anti-aliased edges.
  4. Notification icons should not:
    1. Add alpha (dimming or fading)
    2. Use color
    3. Have opaque backgrounds
    
### Content
1. Base layout
  1. All notifications must include the following elements:
    1. The icon of the originating app
    2. A title and secondary text
    3. A timestamp
  2. Notification type may be included if needed.
2. Expanded layouts
  1. You can choose how much detail your app's notification provides, such as:
    1. The first few lines of a message
    2. A large image preview
    3. A message in its entirety
  2. The user can pinch open or drag to change from a compact layout to an expanded layout.
  3. For individual notifications, Android provides three expanded layout templates: text, inbox, and image.
3. Actions
  1. Android displays actions for common tasks at the bottom of a notification.
  2. Actions should:
    1. Be time-sensitive and meaningful
    2. Suit the content
    3. Allow the user to accomplish tasks
  3. Actions should not:
    1. Be ambiguous
    2. Duplicate the default action (such as "Read" or "Open")
  4. Specifications:
    1. Three actions per notification maximum
    2. Each action has an icon and a name
    3. Actions are visible for expanded notifications, but otherwise hidden
  
### Behavior
1. Notifications are indicated by icons in the status bar, accessible through the notification drawer. Touching a notification opens the associated app. Swiping left or right on a notification removes it from the drawer.
2. Ongoing notifications
  1. Ongoing notifications keep users informed about background processes and provide status for longer tasks, such as file downloads.
  2. A user cannot manually remove an ongoing notification from the notification drawer.
3. Media playback
  1. When an app provides an ongoing notification for active media, users may control playback even when that app is not in the foreground. As notifications are presented on the lock screen, this same experience is available even when the screen is locked.
4. Ranking and ordering
  1. Notifications are shown in reverse-chronological order, with consideration given to the app's stated notification priority.
  2. Notifications are featured prominently on the lock screen and should show the reason for the notification at a glance.
  3. Android sorts notifications according to the following:
    1. The timestamp and application's stated priority
    2. Whether the notification has recently notified the user with a sound or vibration
    3. Any people attached to the notification and whether they are starred contacts
5. Lock screen privacy
  1. Because notifications are visible on the lock screen, user privacy is an especially important consideration. Notifications often contain sensitive information, and should not be visible to anyone who sees the display.
  2. For devices that have a secure lock screen (PIN, pattern, or password), the public version of the interface may be displayed. The private interface is only revealed once the user has signed into the device.
6. User control of secure lock screen information
  1. The user can choose to conceal sensitive details from the secure lock screen, in which case, the system evaluates each notification's visibility level to figure out what can safely be shown.
  2. This setting allows your app to display a redacted version of the content, hiding personal information while still being useful, such as "3 new messages."
  
### Peeking notifications
1. When a high-priority notification arrives, it is presented to users for a short period of time with an expanded layout exposing possible actions. The notification then retreats.
2. If a notification's priority is flagged as High, Max, or full-screen, it gets a peeking notification.
3. Good examples of peeking notifications include:
  1. An incoming phone call when using a device
  2. An alarm
  3. A new SMS message
  4. Low battery
