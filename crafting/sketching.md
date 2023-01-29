# Sketching

FirstStage includes a simple modelling tool for sketching scenery and set dressing. It is inspired by SketchUp.

### Creating a Shape <a href="#_i7apljf5wl9d" id="_i7apljf5wl9d"></a>

To create a shape from scratch, first select the Sketch tool from the Tool WheelMenu.

Draw a path on the ground or any other flat surface by clicking the trigger for each point to form the perimeter of the shape. Close the shape by clicking back on the first point in the path.

While drawing the path, Undo (left on the RadialMenu) will remove the last point placed.

When the path is green, it means that clicking at that point will complete the operation.

When the path is closed, the shape will be created as an extrusion of the polygon created from the path.

**Note:** the path cannot have any crossing lines. When the path is invalid, it will show in red.

### Using Primitives <a href="#_za0mqwsox6mw" id="_za0mqwsox6mw"></a>

You can also start by grabbing a primitive shape from the Asset Store:

* 1m cube
* 1m x 1m x 10cm board
* 1m x 10cm x 10cm post
* 1m x 10cm x 1cm plank

### Editing a Shape <a href="#_b38jq9mse3y9" id="_b38jq9mse3y9"></a>

When you first create a shape it will be immediately editable: you can tell a shape is editable as it will have a blue wireframe showing along with length measurements for the edges and angle measurements for the corners.

If a shape is not editable (as, for example, when a scene is loaded) you can make it editable by holding down the Inspect button and selecting Edit Shape from the Inspect WheelMenu.

### Moving Vertices <a href="#_cojrkc56jaw8" id="_cojrkc56jaw8"></a>

You can highlight a vertex by pointing at it with the Grabber or by pointing at it with your virtual finger. Grab the vertex to move it.

**Note:** moving a vertex may break the planes of surrounding faces at which point the surface will be triangulated with soft internal edges.

### Moving Edges <a href="#_yp1afkshm1s1" id="_yp1afkshm1s1"></a>

Similarly you can grab an edge to move it.

Normally, moving an edge preserves its direction and keeps its vertices locked into the planes of the neighbouring faces. However, an edge can get blocked by its neighbours.

You can unlock the vertices by clicking the grip, and then the vertices will move rigidly with the edge preserving its length. As with moving a single vertex, this may break the planes of neighbouring faces which will force those faces to be triangulated.

You can also grab an edge with two hands which allows you to rotate the edge and the vertices. Clicking the grip in this case will toggle snapping on the rotation angle.

### Moving Faces <a href="#_w6bm88bj0t" id="_w6bm88bj0t"></a>

You can also grab a face to move it.

Normally, moving a face preserves its orientation and preserves the planes of neighbouring faces. This provides a very useful push/pull operation: for example, grab the end face of a wall and drag it to extend the wall. But in conjunction with cutting faces and extrusion, you can create complex geometry easily.

You can also unlock the vertices by clicking the grip, and then the vertices will move rigidly preserving the perimeter of the face. This may break the planes of neighbouring faces in which case those faces will be triangulated.

You can also grab a face with two hands which allows you to both rotate the face (preserving its shape) and scale the face around the centroid. Clicking the grip in this case will toggle snapping on the rotation angle.

### Extruding Faces <a href="#_wly9rkamnyh5" id="_wly9rkamnyh5"></a>

While grabbing a face, press the Extrude button on the RadialMenu to extrude the face: this generates a new ring of faces around the edge of the face; the held face can then be moved freely.

Extruding a face and then scaling it gives a taper effect. You can also extrude inwards to get an inset effect.

You can loft a face along a path by repeatedly extruding it and rotating, translating or scaling it.

### Cutting a Face <a href="#_rn9z2ht9shoz" id="_rn9z2ht9shoz"></a>

If you use the Sketch tool to draw on top of an existing face, you can cut that face and introduce new detail. Such lines will show in cyan instead of orange.

You can split a face by drawing a line from one edge or vertex across a face to another edge or vertex in that face. That line can have multiple vertices but cannot cross itself. The line will show in green when the line ends at a valid cut point.

You can cut a hole in a face by starting a line inside a face and drawing a closed path that doesn’t cross itself or cross any edge of the face.

The most useful thing to do with a hole is to extrude it and push or pull it. If you push an extruded hole all the way to the other side of a shape you can create a tunnel. Note that the tunnel must not intersect any other parts of the shape or you may get an impossible shape.

Tunnels are particularly useful for punching through walls for windows or door.

### Snapping <a href="#_jvb7mh709fd6" id="_jvb7mh709fd6"></a>

By default, snapping works on vertices in World Space. But if a shape is moved, the frame of reference for snapping also moves: this leads to less surprising results when you edit a shape.

However when drawing on a face the snapping is aligned to the UV-space used by the material on that face.

If an edge or face is moved, snapping only happens when the vertices are unlocked.
