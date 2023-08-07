# Parametric Shapes

In the [Asset Library](../basics/asset-library.md), you will find a variety of parametric shapes under the **Shape** tag. You can enable additional handles by choosing the **Edit Shape** option on the [Inspect Menu](broken-reference).

## Cylinder Section

<figure><img src="../.gitbook/assets/DUMMY 2023-02-14 21-13-28.jpg" alt=""><figcaption></figcaption></figure>

* Grab the inside to change the inner radius
* Grab the outside to change the outer radius
* Grab the top or bottom to extend
* Grab the ends to extend the arc of the section

You can also change how the shape is constructed from the [Inspector](../basics/working-with-things/inspector.md):

<table data-header-hidden><thead><tr><th width="220"></th><th></th></tr></thead><tbody><tr><td><strong>Facets</strong></td><td>How many facets to subdivide the curved surface into.</td></tr></tbody></table>

## Sphere Section

<figure><img src="../.gitbook/assets/DUMMY 2023-02-14 21-17-09.jpg" alt=""><figcaption></figcaption></figure>

* Grab the outside to change the outer radi
* Grab the inside to change the inner radius
* Grab one of the edges to change the sweep angle (either latitude or longitude)

You can also change how the shape is constructed from the [Inspector](../basics/working-with-things/inspector.md):

<table data-header-hidden><thead><tr><th width="220"></th><th></th></tr></thead><tbody><tr><td><strong>Facets</strong></td><td>How many facets to subdivide the curved surface into.</td></tr></tbody></table>

## Curved Wall

<figure><img src="../.gitbook/assets/DUMMY 2023-02-14 21-20-44.jpg" alt=""><figcaption></figcaption></figure>

* Grab the spline knots to control the curve of the wall
* Grab the top to change the height
* Grab a side to change the thickness

## Bendable Pole

<figure><img src="../.gitbook/assets/DUMMY 2023-02-14 21-23-41.jpg" alt=""><figcaption></figcaption></figure>

* Grab the spline knots to control the curve of the pole
* Grab with two hands to change the thickness of the pole&#x20;

## Stairs

<figure><img src="../.gitbook/assets/DUMMY 2023-02-14 21-21-51.jpg" alt=""><figcaption></figcaption></figure>

* Grab the spline knots to control the curve of the stairs
* Grab the sides to change the offset from the curve
* Grab the top of the top stair to change the height of the stairs
* Grab the top of the bottom stair to change the height of each step
* Grab the from of a step to change the step length

## Convert to Sketch

Sometimes it can be useful to make more detailed edits than the parametric handles allow. Converting a shape to a sketch allows you to edit vertices, edges, and faces directly and also allowing cutting new faces and extrusion of faces.

To do this, select the shape and go to the [Inspector](../basics/working-with-things/inspector.md) panel on the WristPad and click on the **Convert to Sketch** action.

Note that once converted to a sketch, none of the parametric handles will be available.
