# Lights

There are two types of light in the [Asset Library](../asset-library.md): a basic light which provides a cone spotlight and a beam light which includes some additional VFX to simulate the glow of the beam of a real stage light.

{% hint style="info" %}
Lighting uses Unity's old [Built-In Render Pipeline](https://docs.unity3d.com/Manual/built-in-render-pipeline.html) which most assets on the Unity Asset Store support. FirstStage is planned to support Unity's new [High Definition Render Pipeline](https://docs.unity3d.com/Manual/high-definition-render-pipeline.html) which will allow for physically based lighting.

FirstStage does not yet support realtime global illumination or other techniques to simulate light bouncing between surfaces.
{% endhint %}

Once you've placed a light, you can adjust it from the **Lights** panel on your [WristPad](../wristpad/).

<figure><img src="../../.gitbook/assets/Stage Test2 2023-02-16 16-48-06.jpg" alt=""><figcaption></figcaption></figure>

For each light in the scene, there is a control strip. The first light on the desk is usually the **Sun Light** which is a simple directional light that illuminates the whole scene.&#x20;

Each control strip has a slider to control the intensity of the light. These have a natural range of 0...1 but can be overdriven if desired. But be careful as these are not HDR lights and may well clip badly.

Each strip also has a button to enable automation recording which allows the light to change during the scene.

{% hint style="info" %}
As well as automating the control sliders, you can also animate the position and orientation of the light. Using the [Animator](../core-tools/animator.md) to animate in realtime can be particularly effective as you can keep a spotlight trained on a character, say, as they move around the scene.
{% endhint %}

## Lighting Details

If you click on the header of the light strip, you can open out additional controls:

* Color
* Spot Angle
* Range
* Set whether the light casts shadows

<figure><img src="../../.gitbook/assets/Stage Test2 2023-02-16 16-45-10.jpg" alt=""><figcaption></figcaption></figure>

You can also choose from a wide range of gobos (aka cookies) to put on the light: these can be very useful for simulating many different types of lighting effect.

<figure><img src="../../.gitbook/assets/Stage Test2 2023-02-16 16-45-55.jpg" alt=""><figcaption></figcaption></figure>

The left hand column lists a set of tags for the gobos. Click on a tag to see gobos from that category.

At the top of the tags is a **Clear** button which will remove any gobo from the light.

On the right you can see the gobos: click on one to apply it to the light.
