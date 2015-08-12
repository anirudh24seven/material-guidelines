## Settings

Application settings let users indicate their preferences for how an app or service should behave.

### Usage
1. Settings should be well-organized, predictable, and contain a manageable number of options.       
2. Controls that belong in Settings:
  1. Capture a user preference
  2. Get accessed infrequently
  3. Are used by the majority of users
  4. Are used by a minority of users, but are essential to supporting their needs
3. Items that do not belong in Settings:
  1. Contain information about the app, such as a version number, should move to a Help screen.
  2. Items that manage account actions should appear within the main flow of your app.
  3. Frequently accessed items should move to a toolbar or action overflow menu.
  4. Items used by fewer than 20% of users
  
### Placement
1. Place all Settings under the “Settings” label.
2. Side navigation
  1. If side navigation exists, place Settings below all other items (except Help & Feedback).
3. Navigation drawer
  1. When a navigation drawer is accessible from the current screen, place Settings in the drawer.
4. Apps without navigation
  1. Place Settings in the toolbar action overflow menu below all other items (except Help & Feedback).

### Grouping settings
1. For large lists of settings, cluster settings into multiple shorter lists. Arrange them according to the total number of settings in the Settings panel in your app.
2. 7 or fewer
  1. Don’t group at all.
3. 9 to 10
  1. Group related settings under one or two section dividers. For settings that can't be grouped:
    1. If important, list them at the top without a section divider.
    2. Otherwise, list them at the bottom with a section divider called "Other," in order of importance.
4. 11 to 15
  1. Group related settings under two to four section dividers. Combine sets of two related settings into a single setting.
  2. For example, two related settings with checkboxes could combine into a single multiple-choice setting.
5. 16 or more
  1. Group four or more related settings under a subscreen. Apply the guidance above to each subscreen.
  
### Labels and secondary text
1. Labels
  1. Make your labels brief and meaningful.
  2. Labels should:
    1. Capitalize only the first word of each label, and proper nouns.
    2. Put the most important text of your label first.
    3. Rephrase negative words like "Don't" or "Never" into neutral terms such as "Block."
    4. Use impersonal labels like "Notifications" instead of "Notify me." Exception: If referring to the user is necessary for understanding the setting, use the second person ("you") rather than the first person ("I").
  3. Labels should avoid:
    1. Generic terms, such as: Set, Change, Edit, Modify, Manage, Use, Select, or Choose
    2. Repeating words from the section divider or subscreen title
    3. Technical jargon, unless it's widely understood by your target audience
2. Secondary text
  1. Secondary text is optional. If the label is sufficient on its own, don't add a secondary text description.
  2. Switch or checkbox settings
    1. Settings that require precise descriptions may add a single-line description underneath the settings label.
    2. Descriptions should:
      1. Convey what happens when a setting is enabled
      2. Use words that don't already appear in the label
  3. Settings that require longer explanations may add a description on a second screen.
  4. All other settings
    1. For non-switch settings, secondary text should show the current status of a setting only.
  5. Setting defaults
    1. The initial value for each setting should:
      1. Represent the default most users would choose
      2. Be neutral and pose little risk
      3. Use less battery or mobile data
      4. Only interrupt when important

### Writing guidelines
1. Be direct and understandable.
2. Indicate status with specific details placed within the appropriate context.
3. Use keywords that describe settings accurately.
4. Use familiar acronyms when there aren’t better alternatives. Convey how and why an unfamiliar setting exists.
