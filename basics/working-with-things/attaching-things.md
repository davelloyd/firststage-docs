# Attaching Things

You can show the attachment handle by select **Attach** from the Inspect Menu: it is a sphere at the centre of the thing.

Grab the handle and drag it onto something you want to attach it to: you will see a wire from the attach handle to the target. If the target is a valid thing to attach to, it will highlight yellow and releasing the handle will attach the thing to the target. If not, the target will highlight red.

<figure><img src="../../.gitbook/assets/DUMMY 2023-02-13 12-01-51.jpg" alt=""><figcaption></figcaption></figure>

Some targets may have several distinct locations that you can attach to. Most notably, character puppets can have things attached to their hands, arms, head, chest, legs, feet.&#x20;

<figure><img src="../../.gitbook/assets/DUMMY 2023-02-13 12-04-25 (1).jpg" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Which way you attach things matters. The thing you grab the attach handle from is the child and the thing you attach it to is the parent.&#x20;

Once attached, you can move the child relative to the parent, but moving the parent moves the child as well.
{% endhint %}

## Rigid Attachment

How attachments work depends on what is being attached. Most attachments are rigid: the child will move rigidly with its parent.

For eaxmple you can attach a character to a moving object - say someone hanging on to a car. You can then animate the character relative to whatever the car is doing. This is much easier than trying to keep the character moving with the car (and usually the interpolations don't match up).

Or you can attach a prop to a character to have them, say, wield a gun in their hand, or carry a briefcase, or wear a hat... The possibilities are endless.

Other behaviours for attachment will be desribed where relevant, such as [Camera Follow](../../camerawork/through-the-lens.md#\_6i1r38f850fm).

