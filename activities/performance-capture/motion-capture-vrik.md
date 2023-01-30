# Motion Capture (VRIK)

FirstStage provides a simple but effective form of motion capture inside VR using the headset and controllers to control a character via inverse kinematics (IK). This only really drives the upper body of the character, but the system will try to guess which way you are walking and apply suitable animations to the waist and legs.

You can also use additional Vive trackers attached to your feet (or ankles) and waist to drive them directly.

Note that using trackers and VRIK has some significant limitations: it does not know where your elbows and knees are so has to make a guess. The result usually looks reasonable but may not be what you actually performed. For example, flapping your elbows while keeping hands stationary will not be captured correctly. Human shoulders are actually quite complicated but most puppets do not rig them well, and even if they did, we have no trackers on them so must infer the actual movement.

If you need to capture more subtle performances, FirstStage also supports the Rokoko SmartSuit which uses lots of inertial trackers placed over the body suit to capture many more components of motion. This has different limitations as it can be prone to long chain errors such as clapping your hands where they may not meet correctly in the playback.

### Taking Control of a Puppet <a href="#_bu2qoyq7ae6w" id="_bu2qoyq7ae6w"></a>

To start, point at a puppet with the Navigator (the default left hand tool) when you should see the target teleport destination change to show Take Control over the character’s head. Click & hold the trigger (you’ll see a confirmation timer) and, blink, you’ll be in the Mocap Setup space, a little bubble separate from the rest of the stage.

### Mocap Setup <a href="#_4bmbd0x5pa5z" id="_4bmbd0x5pa5z"></a>

Once in the Mocap Setup space, you’ll see a puppet opposite you which should mirror your actions as you move. If you look down you will also see that you have the puppet as your body.

In front of you is a panel with a choice of motion capture scenarios: one of these is often a good choice.

There are two buttons at the bottom of the middle panel: click on the tick when you are ready to start performing and click on the cross to cancel mocap and go back out to the scene.

To your left is a panel where you can calibrate your height against the height of the puppet which will improve the quality of mocap.

To your right is a panel which gives you fine control of how your performance will drive the puppet.

For your first time, just click the tick and, blink, you’ll be back on set performing inside your character.

### Calibration <a href="#_4fcz81vd21qc" id="_4fcz81vd21qc"></a>

When you first Mocap Setup, you will be asked to calibrate your height by looking at a target in front of you. You can redo this calibration any time by clicking on the **Recalibrate** button.

If you look at your hands, you should see your real hands and the puppet’s hands aligned. Usually this works fine but for some puppets this might not be quite right - particularly those with outsized, cartoony hands. In which case, use your other hand to grab the transparent red sphere which acts as a handle to move the puppet’s hands relative to your hands.

If you are using trackers for your feet and waist, they will also show in the Mocap Setup space and you can also adjust the relative position of your real feet and the puppet’s feet. In practice, you may need to adjust your feet more often as it will depend on where exactly you strapped the trackers to your feet or ankles.

If you are using feet trackers, it is easy to put the left foot tracker on your right foot and vice versa leading to crossed legs. If so, click on the **Swap Feet** button to swap the tracker mapping and you should see your puppet with straight legs.

### Mocap Scenarios <a href="#_uq5dt232xcpl" id="_uq5dt232xcpl"></a>

Depending on what type of performance you are wanting to capture, one of the standard scenarios is a good place to start. The panel on the right will show the details of this selection.

#### Standing <a href="#_by2onydjayvp" id="_by2onydjayvp"></a>

This is the most common scenario: the performer is standing and we want to capture the motion of all body parts.

Any previous animation - either mocap or poses - will be overridden and will not play out during the mocap recording.

If the performer does not have feet and waist trackers, then automatic locomotion will be applied: small steps to keep the puppet’s hips mostly under the puppet’s head.

#### Sitting <a href="#_w9sjx19fdlo8" id="_w9sjx19fdlo8"></a>

Sometimes it is convenient or more comfortable for the performer to sit. For example, the puppet may be posed in a sitting position and we only want to capture the upper body motion. Another case may be where we have animated the puppet moving: if the puppet is moving without the performer’s control this can be very uncomfortable when standing unless you have very good VR legs.

#### Prone <a href="#_8is2gnuznblo" id="_8is2gnuznblo"></a>

This is very similar to the Sitting scenario, except that it does not keep the performer’s head vertical and the head will follow the puppet’s pivot. Be warned, if the puppet is thrown around or is spinning, this can be most uncomfortable!

### Masking <a href="#_r8dvjzj6qwt7" id="_r8dvjzj6qwt7"></a>

If you are layering a performance on top of an existing performance or pose animation, it is useful to turn off those body parts you want to keep from the base layer.

You can select which body parts are driven by clicking on the body mask illustration: head, chest, pelvis, arms, hands, legs & feet.

#### Drive Pivot <a href="#_a2uylfu15moc" id="_a2uylfu15moc"></a>

As well as the pose of the body and limbs, motion capture also records the position and orientation of the body pivot which describes how the puppet moves through space.

Turn this off when layering a performance on top of a base animation that moves the body. Or if the base pose is stationary but you do not want the body to move, for example, when sitting.

### Other Options <a href="#_91ry8v4sapwm" id="_91ry8v4sapwm"></a>

#### Record Speech <a href="#_62hxbgiwlcty" id="_62hxbgiwlcty"></a>

When enabled, speech will be recorded (via the headset mic by default) and appear as a separate track on the timeline. Useful if you want to record placeholder dialogue.

#### Grip Motion <a href="#_isggnap99o50" id="_isggnap99o50"></a>

When enabled, you can move yourself & your puppet using the controller grips as you would outside mocap. This can be useful if you want to rough out someone climbing.

#### Allow Grab <a href="#_dxk7cnl90j2a" id="_dxk7cnl90j2a"></a>

When enabled, you can grab props that have been set as **Holdable** in the Inspector. It is off by default to avoid accidentally picking things up.

#### Walk to Mark <a href="#_n6o1mg7xtpzj" id="_n6o1mg7xtpzj"></a>

When enabled, you can use your off-hand controller to point somewhere to walk to and then press the up button to walk there.

#### Locomotion <a href="#_v75bfgfcmtfk" id="_v75bfgfcmtfk"></a>

When enabled, the puppet will automatically move to keep the pelvis beneath the head as you move around the work area.

Locomotion is automatically disabled if you have feet trackers on.

#### Keep Vertical <a href="#_2lq41qv63ot1" id="_2lq41qv63ot1"></a>

When enabled, the performer will remain vertical in the world regardless of whether the puppet is. Turn this off with caution as it can lead to discomfort if you do not have good VR legs.

#### Lock Work Area <a href="#_lrt2q4rsedml" id="_lrt2q4rsedml"></a>

When enabled, the performer will not be teleported to the puppet at the start of the performance.

This is useful if you have physical props in your work area and want to preserve their alignment to their virtual counterparts in the virtual space.

This is also really useful when you have two performers in the same physical space and want to keep their relative positions. It will also align the work areas to ensure all performers are in the same physical and virtual spaces.

### Physical Props <a href="#_qwpj3jof3aek" id="_qwpj3jof3aek"></a>

It can be useful to have physical props to interact with: for example a performer could put their foot on a cardboard box to match a speaker monitor in the virtual world; or some physical steps could allow the performer to climb virtual stairs.

If you have such physical props, click on the **Mark Physical Props** button to activate the scribble tool. Use this to mark the outlines of physical props: this will now remain fix with respect to your work area.

Cluck on **Clear Prop Scribble** to remove the markup.

### Performing <a href="#_hg4474de3hk2" id="_hg4474de3hk2"></a>

Once you have set up the mocap session as desired, click on the tick button to return to the scene inside the body of your puppet.

Note that recording has not started yet so you have an opportunity to get into position before starting.

### Recording <a href="#_xertxvulriv6" id="_xertxvulriv6"></a>

To start recording, press the up button on the Radial Menu on your main-hand controller. Press it again to stop recording.

You can also press the down button on the Radial Menu to **Retake** the performance: recording is stopped; that performance is discarded; and time rewinds to when you started, ready to have another go.

### Locomotion & Steering <a href="#_i9lt7mhoz7jk" id="_i9lt7mhoz7jk"></a>

If you move around your work area, your puppet will follow you by introducing short animation cycles to take a step in the same direction as you. Generally it will try to keep the pelvis under the head.

However, you often want to go much further than your work area allows. You can steer your puppet much as you would in a game. Steering takes over the puppet from the waist down and plays various walk/run/strafe/turn animation fragments to match where you want to move to.

Push the thumbstick or thumbpad on your off-hand controller forward to walk forwards. You can also push it left or right to strafe or backwards to walk backwards.

Note that the direction your puppet moves is the direction of the controller. This allows your head to look in a different direction to that in which the puppet is walking.

To transition from a walk to a run, click the thumbstick (Index or Oculus) or thumbpad (Vive).

To stop, release the thumbstick or thumbpad.

Normally while steering your puppet, the arms follow the walk or run animations. But if you want to, say, wave while walking you can press the grip button on the controller to take control over that hand again. This also happens naturally if you are holding a prop.

### Grabbing Props <a href="#_s10glb5g2dkj" id="_s10glb5g2dkj"></a>

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

### Linked activities <a href="#_rn76ssp6tnyb" id="_rn76ssp6tnyb"></a>

All activities created during performance capture are linked to the base mocap animation so created. If the base animation is moved, all owned activities are moved with it. If the base animation is deleted, all owned activities are deleted with it.

Such activities include:

* Dialog
* Hold prop
* Use prop

### Finishing the session <a href="#_z4oeqcemfesk" id="_z4oeqcemfesk"></a>

Press both B buttons (Index or Oculus) or Menu buttons (Vive) to leave mocap. This is the same gesture as for going into the Asset Library.
