# Lights

There are two types of light in the [Asset Library](../asset-library.md): a basic light which provides a cone spotlight and a beam light which includes some additional VFX to simulate the glow of the beam of a real stage light.

{% hint style="info" %}
Lighting uses Unity's old [Built-In Render Pipeline](https://docs.unity3d.com/Manual/built-in-render-pipeline.html) which most assets on the Unity Asset Store support. FirstStage is planned to support Unity's new [High Definition Render Pipeline](https://docs.unity3d.com/Manual/high-definition-render-pipeline.html) which will allow for physically based lighting.

FirstStage does not yet support realtime global illumination or other techniques to simulate light bouncing between surfaces.
{% endhint %}

Once you've placed a light, you can adjust it from the **Lights** panel on your [WristPad](../wristpad/): there is a slider strip for each light that lets you control the brightness of the light. Each strip also has a button to enable automation recording which allows the light to change during the scene.

<figure><img src="../../.gitbook/assets/Controls Demo 2023-02-15 01-14-55.jpg" alt=""><figcaption></figcaption></figure>

If you click on the header of the light strip, you can open out additional controls:

* Color
* Spot Angle
* Range
* Set whether the light casts shadows

<figure><img src="../../.gitbook/assets/Controls Demo 2023-02-15 01-15-30.jpg" alt=""><figcaption></figcaption></figure>

You can also choose from a wide range of gobos to put on the light: these can be very useful for simulating many different types of lighting effect.

<figure><img src="../../.gitbook/assets/Controls Demo 2023-02-15 01-15-39.jpg" alt=""><figcaption></figcaption></figure>
