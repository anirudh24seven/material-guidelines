## Swipe to refresh
1. Updating content
  1. There are two methods for updating content in an app. The preferred method is to automatically update content using sync. Syncing keeps app content automatically updated because it doesn’t require user action.
  2. Alternatively, the manual refresh method requires users to initiate content updates via an action or gesture. Manual refreshing can supplement syncing while maintaining a current scroll position, as when checking for new mail in a Gmail account.
2. Swipe to refresh
  1. Swipe to refresh is a swipe gesture available at the beginning of lists, grid lists, and card collections where the most recent content appears (Index 0).
  2. Location:
    1. Typically, this gesture is available at the top of content collections, but it can also be at the bottom (for example, in chat applications).
  3. Usage:
    1. The refresh indicator appears only in conjunction with a refresh gesture or action. Syncing does not display a refresh indicator. It’s best to use this gesture with dynamic content that has frequent updates surfacing from a consistent location, where users have a high probability of seeing new content after initiating the gesture.
    2. Changes may not be immediately obvious to users when this gesture is used in views that can change significantly upon refresh. For example, the refresh may non-sequentially delete, reorder, modify, and insert items or change only off-screen items.
  4. Swipe to refresh should not be used in the following situations:
    1. Navigation drawers
    2. Home screen widgets
    3. Pannable content
3. Refresh indicator positioning and behavior
  1. Position:
    1. The refresh indicator, when resting, is centered horizontally relative to refreshing content.
    2. The refresh indicator is located near the top of refreshing content.
    3. Its exact vertical resting position can be adjusted to promote visual harmony with the underlying layout. For example, the indicator may fall on a material edge or grid line, as long as it’s located near the top of the refreshing content.
  2. Behavior:
    1. As the refresh indicator translates and/or scales into view, the circular spinner fades in while rotating.
    2. The refresh indicator remains visible until the refresh activity completes and any new content is visible, or the user navigates away from the refreshing content.
4. Refresh indicator transitions
  1. When another surface is positioned in front (in z-space) of the material with refreshing content, the refresh indicator translates from underneath that surface and is clipped until it is fully visible.
  2. The refresh indicator scales up in size as it translates when:
    1. The refreshing material is in front of every other surface (in z-space)
    2. A content refresh is initiated via an app bar or overflow menu action
5. Implementation details
  1. To ensure intentional usage of the swipe to refresh gesture, the refresh indicator must pass a threshold before the app will begin to refresh. This threshold is indicated through a number of cues:
    1. The circular spinner reaches 100% opacity.
    2. The rotation of the circular spinner slows down.
    3. The rate of translation of the refresh indicator slows down.
  2. Completing the gesture at any point after passing the threshold will initiate the refresh action.
  3. Reversing the gesture past the threshold will cancel the initiation of the refresh action.
