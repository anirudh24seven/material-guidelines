## Bidirectionality
1. A well-designed app can be easily localized for language scripts that are written and read from left-to-right (LTR), such as English, and for bidirectional language scripts.
2. In bidirectional scripts, text is written and read from right-to-left, but numbers and embedded words from LTR languages, such as non-localized names, are written left-to-right (LTR). Bidirectional scripts include Arabic, Hebrew, and Persian.
3. Bidirectionality affects not only the layout of text and UI elements but also iconography. This section provides basic, high-level information about how to consider bidirectionality in design.

### UI mirroring overview
1. The main difference between left-to-right (LTR) and right-to-left (RTL) interfaces is how the passage of time is articulated. Languages that use LTR scripts depict time as passing from left to right, and languages that use RTL scripts depict time as passing from right to left.
2. Mirroring refers to changing the UI from LTR to RTL or vice-versa, affecting both app layout and graphical elements. Note that the content of text strings, numbers, and embedded words from LTR scripts are not mirrored; they are presented LTR. (The content of text strings are never mirrored; it is always in the correct direction for the language.)
3. The RTL layout is the mirror image of the LTR layout.
4. Key layout changes:
  1. Icons are to the right of text fields.
  2. The navigation buttons are in reverse order.
  3. Icons that communicate direction, like the speaker icon, are mirrored.
  4. Icons that do not communicate direction, such as a camera and a check mark, remain unmirrored.
  5. Text is mirrored, but the clock and phone number are not. Numbers in RTL scripts are displayed LTR.

### RTL mirroring guidelines
1. Follow these guidelines for mirroring text, layout, and iconography to support right-to-left UIs.
2. The guiding principle for RTL interfaces is that time moves from right to left. Forward points to the left, backwards points to the right.
3. The most important icons for mirroring are back and forward buttons.
4. When to mirror
  1. Back and forward navigational buttons are reversed.
  2. An icon that shows forward movement should be mirrored.
  3. Other things are more subtle. For example, an icon that represents a setting uses a slash through the icon to indicate the off state. In an LTR interface, the slash goes from top left to bottom right. In an RTL interface, the slash goes from top right to bottom left.
  4. A volume icon with a slider at its right side should be mirrored. The slider should progress RTL, and the sound waves should emerge from the right.
  5. Icons of people, heads, or faces should typically mirror, especially if they appear close to text. This is so the people face forward, towards the text, instead of backward, shying away from the text. 
    1. This can sometimes be very subtle, as with an angled or slightly turned face, or a grouping of faces.
  6. Sometimes, both the horizontal and circular direction of time are implied in an icon. For example, the redo and undo buttons in Google Docs have both a horizontal direction and a circular direction.
    1. In LTR, these point to the same direction in both circular and horizontal representations of time. In RTL, choose whether to show circular or horizontal direction.
  7. Icons that contain representations of text need careful mirroring.
    1. Text is right-aligned in RTL. If there is a paragraph indent at the beginning of a paragraph, an unfinished line at the end of the paragraph, or a ragged right side, the icons need to be mirrored.
5. When not to mirror
  1. While the linear representation of time is mirrored in RTL, the circular direction of time is not. Clocks still turn clockwise for RTL languages. A clock icon or a circular refresh or progress indicator with an arrow pointing clockwise should not be mirrored.
  2. Some icons refer to physical objects that are not mirrored in the right-to-left world.
    1. For example, physical keyboards look the same everywhere in the world, so they should not be mirrored.
  3. Certain icons might seem directional but they actually represent holding an object with one’s right hand.
    1. For example, the search icon typically has its handle at the bottom right side, because the majority of users are right-handed.
    2. The majority of users in RTL-writing countries are also right-handed, so such icons should not be mirrored.
  4. Media playback buttons and the progress indicator are not mirrored. The LTR direction of these elements represents the direction of the tape, not the direction of time.

### Other localization considerations
1. Text in graphics
  1. Because text in graphical elements will always require localization, try to convey concepts in ways that don’t use text.
2. Numbers
  1. Numbers are also text. Icons containing numbers must be localized for languages that use different numerals. For example, Bengali, Marathi, Nepali, and most Arabic locales use different forms of numbers. An icon containing these numerals would have to be redrawn to accommodate their shape.
  2. Mirroring may be needed even for LTR locales. For example, if one is editing an RTL paragraph inside an English document in Google Docs, the buttons for indenting and lists should be RTL even though the primary UI direction is LTR.
