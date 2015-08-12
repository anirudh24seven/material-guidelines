## Accessibility
1. A product is accessible when all people— regardless of ability—can navigate it, understand it, and use it successfully. Products should aim to be accessible to the widest possible audience.
2. These guidelines are a good starting point for designers who want to learn about accessibility. Designing fully accessible products requires in-depth study. For more info, visit the Google accessibility site.
3. To ensure that your product is usable for those with disabilities, consider what kind of experience users will have by using your product with assistive technologies. Imagine using your product in the following ways:
  1. Without sound
  2. Without color
  3. With high-contrast mode enabled
  4. With the screen magnified
  5. With a screen reader (no visible screen)
  6. With voice control only
  7. With a combination of the above

### Navigation
1. How easy is it to navigate the page quickly and efficiently (e.g. jumping to key sections or getting back to primary navigation)? Present the most important information first. Small changes, like bringing a “create” button to the top, can make navigation much faster.
2. Make touch targets at least 48 x 48 pixels
  1. The recommended minimum touch target size for any element is 48 x 48 dp. Space between elements of your mobile design should be at least 8dp.
3. Support mouse-free and gesture navigation
  1. Are all parts of the design, including every user task and mouseover information, keyboard-accessible on web interfaces and accessible with the basic interaction gestures on mobile devices? Blind users can’t use a mouse to explore your interface in a visual way, instead they will use keyboards to navigate or swipe through elements on mobile devices. Keyboard shortcuts should be consistent with platform standards.
4. Manage navigation between screens
  1. Could a user get lost when navigating between dropdowns, alerts and various screens? Think about how users will return to a screen after closing a dropdown window. Make sure that their focus will return to where it was before the dropdown opened.
  
### Readability
1. Ensure your app is usable with larger font sizes
  1. Is the text still legible when a user magnifies the screen or enlarges the font? Are the essential elements still visible, usable, and not overlapping? Test font adjustments on your app using any of the built-in OS/Browser/App accessibility tools for zooming and viewing large fonts.
2. Ensure critical text has enough contrast
  1. Use a contrast ratio of 4.5:1 between the background and text or critical elements to allow users to read text more easily. Smaller text needs lots of contrast, while big headings can tolerate a wider range of colors and backgrounds.
3. Use more than just color to convey information
  1. This is especially crucial for color-blind users. If colors in a design communicate specific information (e.g., such as the color red representing “high traffic” and the color green representing “no traffic”), it is important to offer an alternate way for the user to get the same information. Combining color with other elements like shapes, patterns, texture, or text can leverage multiple ways to articulate the information.
4. Represent spatial relationships
  1. Is any information conveyed spatially, using layout, that wouldn't be discernable to a blind user who navigates one element at a time? As assistive technologies don't indicate the distance between elements, provide additional clues about how elements are related, such as sharing a common heading.
5. Give visual alternatives to sound
  1. If you have audio elements or system sound alerts, do you provide closed captions, a transcript, or another visual alternative? Any flashing or blinking needs to be translated into a sound, and vice versa.
  
### Guidance and feedback
1. Make interactive controls clear and discoverable
  1. Do all interactive controls have text labels, tooltips, or placeholder text to indicate their purpose? Provide the most relevant information first to the assistive technologies. When naming elements, be consistent in your terminology throughout your app.
2. Provide alternative text for images and video
  1. Are you relying on graphical elements to convey information that isn't also provided in a written format? Do labels provide sufficient semantic context for the task (e.g., not just "download" but "download dinner menu")? Provide alternative text for all images and icons, and avoid using images of text in cases where a standard widget would work.
3. Offer guidance and help
  1. Can the user find help quickly when they do not know what an element means? If a critical element times out, is there a way for the user to reactivate it? Provide clear and easy-to-find contextual help so that the user can look up keyboard shortcuts, gestures, and how to access and use features.
4. Give meaning to links
  1. Some assistive technology modes make navigation more efficient by letting the user scan just the links, ignoring other content. Is the purpose of each link clear? Put the purpose of the link in the link text itself. Generic anchor text like “click here” does not serve this purpose. A better solution is a concrete link, like “Device settings."
