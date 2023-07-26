# Pinning objects

In TAD, you can extrude an object from the ground vertically upwards and paste it to a wall. To extrude objects in all directions, you can pin the objects in TAD.

The concept of pinning is derived from the ancient practice of temple construction in India. Decorative elements like stone pediments were hoisted up and placed onto the walls. Pinning is similar to hanging a painting to a wall. You can extrude an object from the ground and place it on a wall.

**Understanding the Ground Planes dialog box**

Locate the 3D icon bar[![pinning.jpg](https://docs.teamtad.com/\_media/pinning.jpg)](https://docs.teamtad.com/\_detail/pinning.jpg?id=pinning\_objects) on the screen, and click [![pinning\_ed.jpg](https://docs.teamtad.com/\_media/pinning\_ed.jpg)](https://docs.teamtad.com/\_detail/pinning\_ed.jpg?id=pinning\_objects). The following **Ground Planes** dialog box appears.

[![ground\_planes\_pinning\_new.jpg](https://docs.teamtad.com/\_media/ground\_planes\_pinning\_new.jpg)](https://docs.teamtad.com/\_detail/ground\_planes\_pinning\_new.jpg?id=pinning\_objects)

The Ground Planes dialog box displays the following settings:

* **Go to generator object**: The object where the object is pinned is called the **generator object**. Click this button to locate the generator object. The object is pinned to the edge of the generator object that contains the helpers.
* **Ground plane name**: Enter a name for the ground plane.
* **Extrusion details**: Once you locate the generator object, you can see the extrusion details of the pinned ground plane in a box under the ground plane name field. For example, in the above window, the box displays **Extrude outwards of First Floor:BuildingEnvelope**. This means that the extrusion has taken place in the outward direction of the face of object “BuildingEnvelope” in class “First Floor”. The reference point for the pinning is the bottom left corner. The direction of extrusion can be outward or inward with respect to a face of the object.
* **Classes that are pinned onto the ground plane**: All the classes of a particular project can be seen here.

**Method**:

1. Create a new class under **Project** in [the class pane](https://docs.teamtad.com/the\_class\_pane). For instance let's call it “pinned objects”.
2. Create a sub-class under pinned objects and give it a name. For example “xyz”.
3. [Create an object](https://docs.teamtad.com/create\_an\_object) “abc” under sub-class “xyz”. Give it a height in [the site info pane](https://docs.teamtad.com/the\_site\_info\_pane). This height is the measure by which the object is extruded.
4. Open the ground planes window.
5. Enter a name in the ground planes name field.
6. Select the face of the generator object that you want the ground plane to be pinned on.
7. Under “classes that are pinned onto the ground plane” select the class to be pinned.
8. Assign the extrusion properties.
9. Click **Ad**.
10. Click **Ok**.
11. To edit/change the pinned ground plane, click **Ed**.
12. To delete the pinned ground plane, click **De**.

**Note**: In the above example, any objects added to class “xyz” are pinned to the same face of the generator object.

[**Understand pinning more conceptually**](https://docs.teamtad.com/actgpeditor)

***

_Press F1 inside the application to read context-sensitive help directly in the application itself_\
_←_ [_∈_](https://docs.teamtad.com/pinning\_objects?do=edit)\
