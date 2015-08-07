## Chips
1. Chips represent complex entities in small blocks, such as a contact.  They can contain a photo, short title string, and brief information.
2. Chips are manipulated through drag-and-drop. Touching them invokes the full view in a card or full screen view or invokes a menu of options related to that chip’s entity.
3. Animations invoked from chips should resize responsively across views for element persistence.

### Contact chips
1. Contact chips represent contact information that users have for people in a compact way. They are invoked and inserted into a text field (usually the To field) when the user starts typing a contact’s name, sees the contact’s addresses, and selects the correct one. Contact chips can be added directly to a text field from a menu of contacts.
2. Contact chips efficiently confirm that the user will be sending their message to the correct person.
3. Closed contact chip
  1. The contact name text is Roboto Regular 14sp.
  2. Upon focus, the chip rises to an elevation of 2dp. When pressed, it expands to show alternative addresses for the contact.
4. Open contact chip
  1. Contact name text:  Roboto Regular 16sp
  2. Address text: Roboto Regular 14sp
  3. Elevation of the open contact chip is 8dp.
  4. On press, the contact chip closes automatically.
  5. By default, the top field is activated and focused.
