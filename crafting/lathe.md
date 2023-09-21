# Lathe

A lathe object is constructed as a [surface of revolution](https://en.wikipedia.org/wiki/Surface\_of\_revolution) described by a swept spline contour that you can manipulate.

You will find a Lathe in the [Asset Library](../basics/asset-library.md) under **Shape**.

Choose **Edit Shape** from the [Inspect Menu](../basics/working-with-things/#inspect-menu) to manipulate the shape via circular control handles that show in blue wireframe. These move the control points for the swept spline curve. If you click on somewhere there isn't a handle, a new control point will be created there.

<figure><img src="../.gitbook/assets/DUMMY 2023-02-20 17-13-46.jpg" alt=""><figcaption></figcaption></figure>

As well as manipulating the overall shape, you can also change how the shape is constructed from the [Inspector](../basics/working-with-things/inspector.md):

<table data-header-hidden><thead><tr><th width="206"></th><th></th></tr></thead><tbody><tr><td><strong>Curve Smoothing</strong></td><td>Choose between: None, Low, Medium, High.<br><strong>None</strong> will use straight lines between control points.<br><strong>Low, Medium, High</strong> will produce succesively smoother curves between control points.</td></tr><tr><td><strong>Facets per Turn</strong></td><td>Sets how many facets are used around the axis.<br>Small numbers like 3-6 can be used for special effect. <br>High numbers will make for smoother circles.</td></tr></tbody></table>

<figure><img src="../.gitbook/assets/DUMMY 2023-02-20 17-10-28.jpg" alt=""><figcaption><p>A shape with no curve smoothing and only 4 facets per turn (i.e., square).</p></figcaption></figure>
