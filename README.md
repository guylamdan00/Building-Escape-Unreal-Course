# Building-Escape-Unreal-Course
This is a simple escape room game to showcase my current ability in Unreal Engine C++ programing.
The game begins when the player spawns inside a castle, the castle's door is open and the player's goal is *to steal the golden Gargoyle and find a way out of the castle* when the player reach to steal the Gargoyle the door close, and thus begins the player's quest to find the correct items to leave on the Gargoyle's pilllar untill the door open again this time with the golden Gargoyle in his hands.
*Game Mechanics*
The game is built with two basic components; 1)OpenDoor-Applies on a specific door in the room and controls the door movement. When the player begins play the OpenDoor component set the door position in the world and apply the audio component(the door's open and close sound effect) and a PressurePlate(a mass that initiates an event when being hit by a specific actor) onto the door.
When a predetermined weight (unknown to the player) applies to the PressurePlate the door will open using the OpenDoor function and close when the conditions haven't met calling the CloseDoor function.
2)Grabber- apllies on the controller and let the player grab specific actors in the world.
The Grabber-component uses the PhysicsHandle and SetupInput to aplly the mechanics of grab and release onto the controller.
Grab function gets the information needed from the world and player position to initiate a grab event should the conditions specified met.
Release function calls when the conditions specified haven't met.
