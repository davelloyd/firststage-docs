# Posing Characters

Proximity grab a puppet and you can move specific body parts to create poses.

For a humanoid, there are body parts to represent the following bones in the skeleton:

* Chest
  * Head
  * Bicep (Upper Arm)
    * Forearm (Lower Arm)
      * Hand
  * Thigh (Upper Leg)
    * Calf (Lower Leg)
      * Foot

To pose a puppet, with the Grabber selected:

* Move your hand into the puppet until a body part is highlighted in yellow.
* Press and hold the Trigger to grab the body part and move it, then release to set that position.

<figure><img src="../.gitbook/assets/DUMMY 2023-02-10 16-29-46.jpg" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Pose the body parts down the bone hierarchy to avoid having to re-pose body parts that can be affected by the movement of body parts further up the hierarchy.\
E.g/, Move the chest first to create the rough pose, then the bicep, then the forearm, and finally the hand.
{% endhint %}

### Fingers

You can pose fingers the same way. It can be helpful to scale out and make yourself smaller when adjusting fingers.

<figure><img src="../.gitbook/assets/DUMMY 2023-02-10 16-29-56.jpg" alt=""><figcaption></figcaption></figure>

### Moving the Pivot

A puppet's **pivot** is the rigid centre of the puppet, also known as the **root** around which the skeleton articulates.

Whenever you remote grab a puppet, you are always grabbing the pivot.&#x20;

When working close, it is also useful to proximity grab the pivot without stepping back to allow remote grab. In the centre of the pelvis is a sphere handle which you can grab to move the pivot and the whole puppet rigidly.

<figure><img src="../.gitbook/assets/DUMMY 2023-02-10 16-30-04.jpg" alt=""><figcaption></figcaption></figure>

## Animating Poses

Posing a character will create a pose keyframe in an Animate Poses activity. Create an animation by changing time and posing the character again.

{% hint style="info" %}
Use the _Advance a beat_ button on the [Transport Controls](../basics/working-with-time/transport-controls.md) or the [Time Tool](../basics/core-tools/time-tool.md) to move time forward a constant amount (1/2 sec) each time. This can make it much easier to make animations that flow well.
{% endhint %}
