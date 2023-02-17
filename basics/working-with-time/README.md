# Working with Time

Time is a key notion in FirstStage: all animation, automation and other activities are placed on a master timeline.

{% hint style="warning" %}
You can scrub time randomly and the scene will _mostly_ track what you would see with playback forward from the start of the scene. However some behaviours like particle systems have internal state that depends on history and cannot be scrubbed. Other behaviours such as a rotating fan or blinking lights may not be in the same phase on each playback.
{% endhint %}

## Transport Controls

Because time is so important in FirstStage, the [WristPad](../wristpad/) has a set of transport controls at the bottom, which are accessible whichever screen you are looking at. The [Desktop](../using-firststage-on-the-desktop.md) view also has the transport controls at the bottom of the screen.&#x20;

<figure><img src="../../.gitbook/assets/transport controls.png" alt=""><figcaption></figcaption></figure>

From left to right:

* Rewind to start of this section (or whole scene)
* Back a beat (useful for pose animation)
* Forward a beat (useful for pose animation)
* Go to the start of the next section (or end of last activity)
* Play / Pause
* Record / Pause
* Current timeline position
* [Clock synchronisation](../collaboration/#synchronise-clocks) (used when collaborating)
