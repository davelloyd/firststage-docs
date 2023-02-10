# Performing

Once you have set up the mocap session as desired, click on the tick button to return to the scene inside the body of your puppet.

Note that recording has not started yet so you have an opportunity to get into position before starting.

<figure><img src="../../.gitbook/assets/DUMMY 2023-02-10 15-44-43 (1).jpg" alt=""><figcaption></figcaption></figure>

VR inverse kinematics (VRIK) is much like navigating the scene using a game controller. It controls your legs as your navigation hand is dictating the direction the character moves in. If you move around your work area, your puppet will follow you by introducing short animation cycles to take a step in the same direction as you. Generally it will try to keep the pelvis under the head.&#x20;

However, you often want to go much further than your work area allows. You can steer your puppet as much as you would in a game. Steering takes over the puppet from the waist down and plays various walk/run/strafe/turn animation fragments to match where you want to move to.

Normally while steering your puppet, the arms follow the walk or run animations. But if you want to, say, wave while walking you can press the grip button on the controller to take control over that hand again. This also happens naturally if you are holding a prop

1. Using the navigator tool on the tool wheel, via the menu button, point at a character and pull the trigger to 'take control'
2. Once in control, use the ThumbStick (Index or Oculus) or ThumbPad (Vive) on your off-hand controller to move your character in a full 360 degrees range of movement.
3. If you want to speed the pace your character moves into a **jog**, click the ThumbStick (Index or Oculus) or ThumbPad (Vive) once. If you want your character to move into a swift **run** press the ThumbStick (Index or Oculus) or ThumbPad (Vive) twice.

_Tip: Physically move your body to change direction._

_Note: The direction your puppet moves is the direction of the controller. This allows your head to look in a different direction to that in which the puppet is walking._

## Recording <a href="#_xertxvulriv6" id="_xertxvulriv6"></a>

To start recording, press the up button on the Radial Menu on your main-hand controller. Press it again to stop recording.

You can also press the down button on the Radial Menu to **Retake** the performance: recording is stopped; that performance is discarded; and time rewinds to when you started, ready to have another go.

## Locomotion & Steering <a href="#_i9lt7mhoz7jk" id="_i9lt7mhoz7jk"></a>

If you move around your work area, your puppet will follow you by introducing short animation cycles to take a step in the same direction as you. Generally it will try to keep the pelvis under the head.

However, you often want to go much further than your work area allows. You can steer your puppet much as you would in a game. Steering takes over the puppet from the waist down and plays various walk/run/strafe/turn animation fragments to match where you want to move to.

Push the thumbstick or thumbpad on your off-hand controller forward to walk forwards. You can also push it left or right to strafe or backwards to walk backwards.

Note that the direction your puppet moves is the direction of the controller. This allows your head to look in a different direction to that in which the puppet is walking.

To transition from a walk to a run, click the thumbstick (Index or Oculus) or thumbpad (Vive).

To stop, release the thumbstick or thumbpad.

Normally while steering your puppet, the arms follow the walk or run animations. But if you want to, say, wave while walking you can press the grip button on the controller to take control over that hand again. This also happens naturally if you are holding a prop.

## Grabbing Props <a href="#_s10glb5g2dkj" id="_s10glb5g2dkj"></a>

While performing as a puppet, you can grab a prop by moving your hand close to it (the prop will highlight) and then press and hold the grip button on that controller.

Let go of the prop by releasing the grip button: the prop will then move under physics, falling to the ground. If you let go while performing a throwing motion, that velocity will be imparted to the prop giving a throwing action. However, the lack of any weight and tactile feedback in VR means this is not very accurate and can take a little practice to achieve the desired result.

Note that unlike the Grabber tool which uses the trigger button, this uses the grip button. This allows the trigger to be used for the Use action if the prop has one.

Such a prop must be flagged as **Holdable** in the Inspector.

Held props will collide with scenery and may be blocked by them.In which case you will see the puppet’s hand still following the prop even if your controller is not. For example, if you are holding a mug and put it down on a table, the mug will hit the table and not move through it; your puppet’s hand will remain attached to the mug even if your controller is now well below the table.

#### Hand Pose <a href="#_mpovb6qfqqey" id="_mpovb6qfqqey"></a>

If a prop has a **Hand Pose** attached to it, the puppet’s hand will move to meet that hand pose (and the thing will also spring to match the incoming hand). This helps compensate for the lack of tactile feedback in VR which makes it hard to locate hand and fingers naturally for holding a thing.

#### Using a Prop <a href="#_hj8cn7uo3sn8" id="_hj8cn7uo3sn8"></a>

Some props are rigged to be **Useable**: often this is done inside the Unity editor before importing to FirstStage but it also also possible to create such a ‘hero’ prop inside FirstStage (see ????).

To use a prop, pull the trigger. For continuous actions (for example, a fire extinguisher) keep holding the trigger and release when done.

As an example try the **Handgun M1911A** which fires a bullet when the trigger is pulled.

## Linked activities <a href="#_rn76ssp6tnyb" id="_rn76ssp6tnyb"></a>

All activities created during performance capture are linked to the base mocap animation so created. If the base animation is moved, all owned activities are moved with it. If the base animation is deleted, all owned activities are deleted with it.

Such activities include:

* Voice clip
* Hold prop
* Use prop

## Finishing the session <a href="#_z4oeqcemfesk" id="_z4oeqcemfesk"></a>

Press both B buttons (Index or Oculus) or Menu buttons (Vive) to leave mocap. This is the same gesture as for going into the Asset Library.
