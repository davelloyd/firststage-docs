---
description: 12th July 2018
---

# Release 10

## Update (a)

* Prototype Collaboration support:
  * Users in the same scene should be able to see each other (if in VR) and talk to each other.
  * If a user makes a change to a scene, other users in the scene will see the result.
* If you open a scene without saving (going back to the Office), any changes since last save should be preserved

_Note: the Airbrush does not yet save brush strokes so painted sketches must be saved or will be lost (WIP)_

_Note: there are still issues with connectivity and NAT traversal – users should be able to connect directly to a host on the same LAN but for remote users it will depend on the network firewall._

* Prototype desktop UI for viewing through cameras and playing back a scene (WIP):
  * There is a Timeline at the bottom of the screen with basic transport controls.
  * On the left hand side there are icons for cameras, remote users and smartsuits.
  * Click on a camera to see its current viewpoint.
* Click on a remote user to see an ‘over the shoulder’ view of what they’re doing.
* Timeline now provides transport controls as an alternative to the Time Tool.
* Sketches now show measurements along their edges when handles are visible – can be disabled globally from the Sketch Palette on the WristPad
* Puppet IK handles are now hidden by default. Use the top radial button on the Hand tool to reveal. IK paths are only shown when handles visible.
* Trigger on Navigator teleports again – use as secondary grab proved confusing.
* Leaving Camera TTL view should now return you to where you were.
* Zooming is disabled in the Office
* Controller pointers should be less jittery particularly when sketching.
* Performance improvements to reduce frame stutters – should be much smoother in VR

## Update (b)

* Teleporting now preserves your scale and no longer resets it to normal.
