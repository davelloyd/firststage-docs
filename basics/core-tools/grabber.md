# Grabber

The Grabber is the tool for picking up things and placing them. It is the default tool on your main hand.

Simply point the beam at something and pull the trigger to pick it up and move it. The grabber uses physics to move things which helps to place things clean on or next to other things. It will resist objects interpenetrating, but if you keep moving something through something else, it will allow it.

Click the grip button to toggle grid snapping on or off. Go to the [Settings](broken-reference) panel on the [WristPad](../wristpad/) to change the snap settings.

{% hint style="info" %}
Not everything can be moved. It may be **Locked** and need unlocking from the Inspector or be part of the background stage.
{% endhint %}

## Radial Menu

* Undo
* Redo
* Drop to ground (keep holding the trigger until the thing has landed and stopped moving)
* Pull to hand (useful if a thing is far away)

## Proximity Grabber

As well as grabbing things from a distance, you can also grab things by reaching out your hand directly: the hand will turn solid and you can grab the thing.

The proximity grabber will trigger whenever your hand is touching something else, regardless of which tool was selected. This is particularly useful when working with other tools such as the Sketcher as you can just grab the handles without switching between the Sketcher and the Grabber.
