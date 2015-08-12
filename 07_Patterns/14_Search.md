## Search

### In-app search
1. When an app supports large amounts of information, users should be able to quickly locate content by searching.
2. Basic search involves:
  1. Opening a search text field
  2. Entering and submitting a query
  3. Displaying a set of search results
3. However, the search experience can be enhanced by providing:
  1. Voice search
  2. Historical search suggestions based on recent user queries, before a query is completed
  3. Auto-completed search suggestions matching actual results in your application data
4. There are two major patterns for in-app search: persistent search and expandable search.
5. Persistent search
  1. Use persistent search when search is the primary focus of your app.
  2. Behavior:
    1. The search text field is presented inside of an inset search box, ready to receive focus. The user can touch the microphone icon to initiate a voice search.
    2. When in focus, the search field expands to show historical search suggestions. If needed, the onscreen keyboard will also appear.
    3. Choosing any of the suggestions submits the search. Touching the up arrow releases the focus from search, dismissing suggestions and the on-screen keyboard.
    4. As the user enters a query, the search suggestions shift to auto-completion. As the user types, the suggestions are filtered and sorted. Choosing a suggestion or pressing the return key submits the search.
    5. The X action in the search box clears the query.
    6. When displaying search results, the search box remains visible, but is not focused by default. The onscreen keyboard is dismissed so more results can be shown.
    7. Search results are formatted as cards to match the inset appearance of the search box and to accommodate different types of results.
6. Expandable search
  1. Use expandable search when search is not the primary focus of your app.
  2. Behavior:
    1. Display a magnifying glass icon in the toolbar instead of a search text box.
    2. Touching the search icon causes the toolbar to transform, clearing other content and displaying a search text field. If voice search is supported, the microphone icon also appears.
    3. The search text field automatically receives focus, and, if needed, the onscreen keyboard will appear. Historical search suggestions can be shown beneath the toolbar. Choosing any of the suggestions submits the query.
    4. Touching the up arrow closes search and restores the original presentation of the toolbar.
    5. As the user enters a query, the search suggestions shift to auto-completion. As the user types, the suggestions are filtered and sorted. Choosing a suggestion or pressing the return key submits the search.
    6. The X action in the search field clears the query.
    7. When displaying search results, the search version of the toolbar remains visible, but is not in focus by default. The onscreen keyboard is dismissed so more results can be shown.
    8. Search results are formatted as cards and appear in the main body of the page beneath the toolbar.
