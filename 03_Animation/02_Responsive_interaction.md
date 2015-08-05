## Responsive interaction
Responsive interaction encourages deeper exploration of an app by creating timely, logical, and delightful screen reactions to user input. Each interaction is thoughtful, perhaps whimsical, but never distracting. What will happen if I touch this screen? And then this icon?

### User input
1. In material design, apps are responsive to user input:
  1. Touch, voice, mouse, and keyboard are all equally important input methods.
  2. UI elements appear tangible, even though they are behind a layer of glass (the device screen). To bridge that gap, visual and motion cues acknowledge input immediately and animate in ways that look and feel like direct manipulation.
2. Responsive interaction elevates an app from an information-delivery service to an experience that communicates using multiple visual and tactile responses.

### Surface reaction
1. Upon an input event, the system provides instant visual confirmation at the point of contact: under the pad of a finger for touch, at the microphone for voice, or in the appropriate field for a keyboard press.
2. The core visual mechanism to express this contact is the Touch Ripple. This device articulates the method and duration of a touch event, as well dynamic variables like voice amplitude or touch pressure.
3. Best Practices
  1. From the point of input (the contact point of a finger or the microphone icon for voice), make the visual reaction radial.
  
### Material response
1. In addition to ink-like surface reactions, material can lift up when touched, indicating an active state. On touch, the user can generate new or transform existing material, or directly manipulate sheets of material by dragging or flinging them. Material can be resized linearly or radially.
2. Point of origin
  1. When a user triggers the creation of new material, it should grow in size starting from the point of input.
3. Lift on touch
  1. When a card or separable element is activated, the card should lift to indicate an active state.

### Radial action
1. Add clarity to user input through visual reactions to user input. Radial action is the visual ripple of ink spreading outward from the point of input.
2. Input events are visual
  1. The connection between an input event and on-screen action should be visually represented to tie them together. For touch or mouse, this occurs at the point of contact. For voice, the microphone icon. A touch ripple indicates where and when a touch occurs and acknowledges that the touch input was received.
3. Connect input to action
  1. Transitions, or actions triggered by input events, should visually connect to input events. Ripple reactions near the epicenter occur sooner than reactions further away.
  2. For example:
    1. A sequence of content changes: images fade in or out.
    2. A sequence of material movements: cards enter on or off the screen.
