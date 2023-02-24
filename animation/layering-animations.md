# Layering Animations

Partial MoCap using 'VRIK animation' controls and imitates the lower part of the body. Without full MoCap, it is essential to layer animations using different animation methods to build up your puppets action within the scene. Not only does this allow for a better quality of animation, but it ensures you can access every detail of your scene, and the best part is , you never have to leave your seat!

Starting with VRIK animation, you can add upper body movement by posing body parts, partial mocap and puppet animation. To add audio and facial expressions, use 'Facial Capture'.

For example, to get a policeman to pull out a gun after a chase;

* Use VRIK animation to steer the animation create movement of the legs.
* Change the mocap control of body parts to the upper body, by turning the **pivot off** and turning on the arms of the puppet in the mocap setup room. Scrub to the time you want to draw the gun and record the action of you physically doing it.
* You will see them as seperate keyframes associated with the same character on the timeline that you are easily able to manipulate in order to complete the desired action in the scene.
* Add a gun and use proximity grab to pose the characters fingers around it.
* Make sure you attach the gun using the 'attach handle' to the hand. Firststage will construct the drawing of the gun out the holster for you, if the gun is attached.

_Note: Turn off the pivot in order to layer upper body mocap ontop of the lower body VRIK._
