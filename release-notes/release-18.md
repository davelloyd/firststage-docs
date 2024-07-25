---
description: 17th June 2019
---

# Release 18

## Physics

* Synthesizing animation with rigid body physics and ragdolls has been much improved (yet there is still much to do).
* You can enable physics from the Inspector panel on the WristPad.
* When physics is enabled, things will collide with each other and bounce off each other.
* Puppets also have simple physics behaviour and their limbs may be deflected by obstacles. In extremis they may fall into unpinned ragdoll behaviour.

### **Fractures**

* You can also enable fractures from the Inspector panel on the WristPad.
* In this case, when it collides with something it will break into a number of shards. The style of breakage is that of pottery or plaster. The resulting shards will then move rigidly bouncing and flying round the scene.
* Note there may be a brief lag between impact and the shards appearing as this is calculated at runtime and may take a few frames.

### **Vehicles**

* Vehicles have been revived from an early prototype. There is only one drivable vehicle so far in the asset repository: the Unity Car.
* You can mark out a path for a vehicle to follow just like a puppet.
* Vehicles also have physics when driven so will collide with obstacles and knock them out of the way if they also have physics enabled.
* You can also Take Control of a vehicle. While inside the vehicle, the right controller’s trigger is the accelerator and the left controller’s trigger is the brake. There is also a handbrake on the left controller’s thumbpad. You steer the vehicle by moving the controllers. While the vehicle is being driven, it’s path is recorded and time advances.

### **Concave Colliders**

* Most of the time FirstStage treats passive props as boxes which makes their behaviour under physics unrealistic. It can also make placing assets awkward as they bump up against the extents of nearby props.
* First Stage now supports NonConvexColliders which breaks a concave collider down into a smaller set of convex colliders. It uses the well regarded V-HACD algorithm.
* Assets must be re-imported to enable concave colliders (the standard assets will be re-imported shortly) – there will be a new release of RepoMan to allow this.

### **Repeatability**

* Physics is not very repeatable! Collisions rarely happen the same way twice although they will be similar. However divergence of outcomes increases the more bounces occur so that frequently each take will be quite different in detail.
* Thus, physics is most appropriate for incidental animation – fractures being a good example as we rarely care what shape shards we get.

## Commenting

* To help with collaborative working, First Stage now includes a commenting system that allows users working in a scene to communicate with each other in an offline and asynchronous fashion. This can be found on the Chat (formerly Collaboration) panel from the WristPad.

### **Attaching comments to Things**

* Select multiple things with the Selection Tool and then go to the Inspector on the WristPad.
* Click on the Record Comment button (bottom right) and then dictate your comment. Click on the Record Comment button again to stop recording.
* Go to the Chat panel on the WristPad to see all the comments recorded in the scene. The interface is similar to Slack, Skype and such: each comment shows who made it and when, along with a list of the Things referenced. Press the Play button to listen to the comment.
* If you have Speech Recognition enabled (Windows 10 only), you will also see a transcript of the the message. The quality of the transcript is often poor but can be improved by training it to your voice.

### **Photos**

* You can also attach a photo to a comment. Click on the Camera button to summon the Viewfinder. In this mode you can only take a still image but it otherwise works as normal.

### **Scribbles**

* As well as recording a voice message, you can grab a virtual marker pen from the Collaboration panel (bottom right icon) and scribble in the scene. This allows you to illustrate motion, outline changes, sketch an idea, etc.
* You can choose the colour of the marker from the Airbrush Palette.
* Each group of pen strokes is presented as a comment on the Collaboration panel.
* You can hide (or show) all scribbles from the Preferences panel on the WristPad.

## Saving assemblies as Assets

* Select multiple things with the Selection Tool and then go to the Inspector on the WristPad.
* Click on the Save as Asset button (bottom left). You will be flipped into the Office with a form in front of you. Here you can give the new asset a name, tags and a description.
* Once saved as an asset, it will be available in the Browser and then be instantiated in the scene as many times as you want.

### **Project Assets**

* First Stage now distinguishes assets that are specific to a Project from public assets that are available to anyone. Assemblies are saved as project assets. A new version of the Repo Man will upload assets to specific projects.
* To find project assets, click on the Project Assets button in the Asset Browser.

## Other Changes

* Things can now be locked via a switch in the Inspector: once locked they cannot be moved or manipulated until unlocked.
* Activities can now be muted on the timeline: click on the tick by the activity description to toggle. Muted activities do not do anything. This allows you to try different ideas or takes.
* Snapping on sketches has been improved. The line will now show green when snapped to the start forming a closed loop.
* The near plane can now be set in the Camera TTL view.
