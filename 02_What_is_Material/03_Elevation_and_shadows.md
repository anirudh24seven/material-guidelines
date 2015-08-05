## Elevation and shadows
1. Objects in material design possess similar qualities to objects in the physical world. In the physical world, objects can be stacked or affixed to one another, but cannot pass through each other. Objects cast shadows and reflect light.
2. These qualities form a spatial model that is familiar to users and can be applied consistently across apps. Underpinning this spatial model are the concepts of elevation and shadow.

### Elevation (Android)
1. Elevation is the relative depth, or distance, between two surfaces along the z-axis.

  1. Elevation is measured in the same units as the x and y axes, typically in density-independent pixels (dp). Because material elements have depth (all material is 1dp thick), elevation is measured in distance from the top of one surface to the top of another.
  
  2. A child object's elevation is relative to the parent object's elevation.
  
  
2. Resting elevation

  1. All material objects, regardless of size, have a resting elevation, or default elevation that does not change. If an object changes elevation, it should return to its resting elevation as soon as possible.
  
  
3. Component elevations:

  1. The resting elevation for a component type is consistent across apps (e.g., FAB elevation does not vary from 6dp in one app to 16dp in another app).
  
  2. Components may have different resting elevations across platforms, depending on the depth of the environment (e.g., TV has a greater depth than mobile or desktop).
  
  
4. Responsive elevation and dynamic elevation offsets:

  1. Some component types have responsive elevation, meaning they change elevation in response to user input (e.g., normal, focused, and pressed) or system events. These elevation changes are consistently implemented using dynamic elevation offsets.
  
  2. Dynamic elevation offsets are the goal elevation that a component moves towards, relative to the component’s resting state. They ensure that elevation changes are consistent across actions and component types. For example, all components that lift on press have the same elevation change relative to their resting elevation.
  
  3. Once the input event is completed or cancelled, the component will return to its resting elevation.

  
5. Avoiding elevation interference:

  1. Components with responsive elevations may encounter other components as they move between their resting elevations and dynamic elevation offsets. Because material cannot pass through other material, components avoid interfering with one another any number of ways, whether on a per-component basis or using the entire app layout.
  
  2. On a component level, components can move or be removed before they cause interference. For example, a floating action button (FAB) can disappear or move off-screen before a user picks up a card, or it can move if a snackbar appears.
  
  3. On the layout level, design your app layout to minimize opportunities for interference. For example, position the FAB to one side of stream of a cards so the FAB won’t interfere when a user tries to pick up one of cards.
  

### Shadows
1. Shadows provide important visual cues about objects’ depth and directional movement. They are the only visual cue indicating the amount of separation between surfaces. An object’s elevation determines the appearance of its shadow.
2. In motion, shadows provide useful cues about an object’s direction of movement and whether the distance between surfaces is increasing or decreasing.
3. Component reference shadows:

  1. App bar - 4dp
  
  2. Raised button - Resting state: 2dp, Pressed state: 8dp
  
  3. Floating action button (FAB) - Resting state: 6dp, Pressed state: 12dp
  
  4. Card - Resting state: 2dp, Picked-up state: 8dp
  
  5. Menus and sub menus - Menus: 8dp, Sub menus: 9dp (+1 dp for each sub menu)
  
  6. Dialogs: 24dp
  
  7. Nav Drawer & Right drawer - 16dp
  
  8. Bottom sheet - 16dp
  
  9. Refresh indicator - 3dp
  
  10. Quick entry/Search bar - Resting state: 2dp, Scrolled state: 3dp
  
  11. Snackbar - 6dp
  
  12. Switch - 1dp
  
### Object relationships
1. Object hierarchy

  1. How you organize objects, or collections of objects, in an app determines how they move in relation to one another. Objects can move independently of each other or be constrained by objects higher in the hierarchy.
  
  2. All objects are part of a hierarchy described in terms of a parent-child relationships. The “child” in each of these relationships refers to an element that is a subordinate to its “parent” element. Objects can be children of either the system or another object.
  
  3. Parent-child specifics:
    
    1. Each object has one parent.
    
    2. Each object may have any number of children.
    
    3. Children inherit transformative properties from their parent, such as position, rotation, scale, and elevation.
    
    4. Siblings are objects at the same level of hierarchy.
    
2. Exceptions

  1. Items parented to the root, such as primary UI elements, move independently of other objects. For example, the floating action button does not scroll with content. 
  
  2. Other elements include:
  
    1. An app’s side nav drawer
    
    2. The action bar
    
    3. Dialogs
  
3. Interaction

  1. How objects interact with one another is determined by their place in the parent-child hierarchy.
  
  2. For example:
  
    1. Children have minimal z-axis separation from their parent; other objects do not get inserted between parents and children.
    
    2. In a scrolling card collection, the cards are siblings of each other, so they all move together in tandem. They are children of the card collection object that controls their movement.
    
4. Elevation
  1. How you determine the elevation of objects—their position in z-space—depends on the content hierarchy you want to express and whether an object needs to move independently of other objects.
    
