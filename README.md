I wanted to have a "template" project configured for godot so I wouldn't have to go through all of the setup steps each time I started a new project. godot itself doesn't let you do this, so I created this project as a starting point for any new project. It will start you out with the following:

- The base project in Compatability Mode, which is what is recommended for VR experiences aimed specifically at the Quest.
- A "main" scene already prepared with:
  - World Environment turned on
  - Directional Light turned on
  - An XROrigin3D object that is the player perspective
  - A solid Floor object with a little space to move around
  - A Table object
  - A Block object that can be picked up
- An "xrOrigin" scene that contains all of the controls used by the player, including:
  - XRCamera3D which will be the players view
  - A LeftHand object that controls player movement on the left joystick (MovementDirect) and can be used to pick up objects (FunctionPickup)
  - A RightHand object that controls player turning on the right joystick (MovementTurn) and can be used to pick up objects (FunctionPickup)
- A "pickable_block" scene that contains controls for how the players interacts with the Block object, including:
  - A GrabPointHandLeft and GrabPointHandRight object to add animation to the grab action on both hands

This template project is also already preloaded with 3 plugins:

- Godot XR Tools, which provide all of the basic functionality needed for a VR experience.
- GameDev Assistant, which provides an AI coding assistant from Zenva.
  - I currently only have the free version of this plugin which has a limited number of questions that can be asked per month. If we find we use this tool a lot I can get the Pro version.
- Terrain3D, which has tools for "painting" terrain for a VR scene.

All of the plugins are enabled and my GameDev Assistant API key should already be saved with the plugin information.
