## Gestures
1. Mobile only
2. Gestures are divided into Touch Mechanics (what your fingers do on the screen) and Touch Activities (results of specific gestures).  
3. A touch mechanic (such as swipe) may have multiple results (such as enable/disable), depending on the context. A touch activity (zoom in) may be achieved through multiple touch mechanics (pinch open, double touch, etc.).
4. The Drag, Swipe, and Fling touch activities are covered in more detail due to their highly contextual results.

### Touch mechanics
Touch mechanics refer to what the user's fingers do on the screen.

1. Touch
  1. One-finger press, lift
  2. Example: Select
2. Double touch
  1. One-finger press, lift, one-finger press, lift
  2. Example: Zoom in
3. Drag, Swipe, or Fling
  1. One-finger press, move, lift
  2. Example: Dismiss, scroll, tilt, etc.
4. Long press
  1. One-finger press, wait, lift
  2. Example: Select an element, such as a list item
  3. Long press is not used to display a contextual menu.
5. Long-press drag
  1. One-finger press, wait, move, lift
  2. Example: Pick up and move, select multiple items
6. Double-touch drag
  1. One-finger press, lift, one-finger press, move, lift
  2. Example: Zoom in, zoom out
7. Pinch open
  1. Two-finger press, move outwards, lift
  2. Example: Zoom in
8. Pinch closed
  1. Two-finger press, move inwards, lift
  2. Example: Zoom out
9. Two-finger touch
  1. Two-finger press, lift
  2. Example: Zoom out
10. Two-finger swipe, drag, fling
  1. Two-finger press, move, lift
  2. Example: Select multiple items, pan, tilt
11. Two-finger long-press
  1. Two-finger press, wait, lift
  2. Example: None; this gesture is uncommon.
12. Two-finger long-press drag
  1. Two-finger press, wait, move, lift
  2. Example: Pick up and move
13. Two-finger double touch
  1. Two-finger press, lift, two-finger press, lift
  2. Example: Zoom out
14. Rotate
  1. Two-finger press, simultaneously orbit both fingers around the center point, lift
  2. Example: Rotate content, such as a map
    
### Touch activities
Specific gestures and their results, in context.

1. Activate
  1. Activates a screen element, like a button
  2. Touch
2. Cancel or Escape
  1. Cancels or escapes out of the current task, as in dialogs or menus
  2. Touch
3. Enable/Disable lights out
  1. Hides or shows a view’s chrome
  2. Touch
4. Drag or Swipe or Fling
  1. See the following section Drag, swipe, or fling details for distinctions between Scroll, Reveal upon scroll, Pan, Dismiss, Swipe to refresh, Edge swipe, Paging swipe, Overscroll collapse, Menu open, and Tilt
  2. Drag, Swipe, or Fling
5. Data selection (when nothing is selected)
  1. Selects a single element
  2. Long press, two-finger touch
6. Data selection (when items are already selected)
  1. Selects additional elements while in selection mode 
  2. Can use any combination of subsequent one- or two-finger gestures
  3. Touch, two-finger touch
7. Data multi-selection drag
  1. Reveals selection box that originates from point of gesture initiation
  2. The height and width can be adjusted based on finger position. 
  3. The final selection is based on selection box dimensions upon finger(s) lifting.
  4. Two-finger swipe or drag, long-press drag with no items selected
8. Pick up and move
  1. Affects the selected item or items. It can be used to:
    1. Rearrange data within a view
    2. Move an item into a container or onto a target
    3. Reorder items in a list or a card collection
  2. Two-finger long-press drag, long-press drag on selected item
9. Zoom in
  1. Scales up content
  2. Touch Mechanics
    1. Double-touch
    2. Double-touch drag (down)
    3. Pinch open
10. Zoom in to fit
  1. For nested views, scales up the smallest targetable view
  2. Double-touch
11. Zoom out
  1. Scales down content
  2. Touch mechanics:
    1. Double-touch at maximum zoom
    2. Double-touch drag (up)
    3. Pinch closed
    4. Two-finger touch
    5. Two-finger double touch        
12. Expand
  1. Expands collapsed content
  2. Pinch open
13. Collapse
  1. Collapses expanded content
  2. Pinch closed
14. Rotate
  1. Rotates the targeted content
  2. Rotate

### Drag, swipe, or fling details
1.  Swipe gesture activities vary based on context. The speed at which a gesture is performed is the primary distinction between Drag, Swipe, and Fling.
  1. Drag: Fine gesture, slower, more controlled, typically has an on-screen target
  2. Swipe: Gross gesture, faster, typically has no on-screen target
  3. Fling: Gross gesture, with no on-screen target
2. Gesture velocity impacts whether the action is immediately reversible.
  1. A swipe becomes a fling based on ending velocity and whether the affected element has crossed a threshold (or point past which an action can be undone).
  2. A drag maintains contact with an element, so reversing the direction of the gesture will drag the element back across the threshold.
  3. A fling moves at a faster speed and removes contact with the element while it crosses the threshold, preventing the action from being undone.
3. Scroll
  1. A scroll is a vertical or horizontal swipe in a single direction within the content body.
  2. Usage
    1. Scroll amount varies based on velocity of gesture: drag (slow) vs. swipe vs. fling (fast).
    2. Scrolled content should move at the same rate as the gesture being performed. The content should feel "anchored" to the finger or touch device.
4. Reveal upon scroll
  1. Reveal upon scroll means that reversing the scroll direction in a content area reveals hidden in-app elements. E.g., scrolling up in Chrome shows the Omnibox. To dismiss these in-app elements, resume the original scroll direction.
5. Pan
  1. A pan is an omnidirectional one- or two-finger gesture that expands the field of view. Drag is typically used with pan. Fling will maintain gesture velocity, resulting in a significant pan of the content along the direction of the fling gesture.
  2. Pan is applied to:
    1. Unbounded content (maps)
    2. Content that is larger than the screen height or width (zoomed in web page or photo)
  3. A two-finger pan occurs when transitioning from another two-finger gesture (e.g., pinch zoom or rotate) such as in Maps. When a gesture begins with a two-finger pan it results in tilt.
6. Dismiss
  1. A dismiss gesture originates on a swipeable element, such as a list item or card, orthogonal to the direction of scrolling.
  2. The gesture is typically horizontal.
  3. The dismiss gesture is committed based on crossing a threshold.
7. Swipe to refresh
  1. Swipe to refresh usually occurs in a vertical and downward movement. It is available at the top of a list, or at the edge of any card or container where new content surfaces.
8. Edge swipe
  1. An edge swipe gesture originates outside of the screen to reveal off-screen content. It invokes content separate from the current view.
  2. If no edge swipe action is defined, an edge swipe can default to a paging swipe.
  3. The edge swipe gesture is committed based on crossing a threshold.
9. Paging swipe
  1. A paging swipe is an on-screen, in-content swipe that reveals related off-screen content. It reveals one page/tab per paging swipe.
  2. If paged content is at >100% zoom, an in-content swipe will Pan to an edge of the content, and an additional in-content swipe will Page.
  3. The Paging swipe gesture is committed based on crossing a threshold.
  4. Don’t use paging swipes when individual elements are swipeable.
  5. See below: Overscroll collapse
10. Overscroll collapse
  1. Overscroll collapse navigates up in the content hierarchy via a paging swipe at the top or bottom of scrolling content.
  2. The Overscroll collapse gesture is committed based on crossing a threshold.
11. Menu open
  1. A drag originating from a menu or picker reveals a menu. Upon lift, the highlighted menu option is selected.
  2. The menu then appears upon touch.
  3. Drag is used with Menu open.
12. Tilt
  1. Tilt moves 3D content forward or backward.
  2. The transition from another two-finger gesture (e.g., pinch zoom or rotate) such as in Maps, will result in a two-finger pan.
  3. Drag is used with Tilt.
