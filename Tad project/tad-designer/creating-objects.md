# Creating Objects

You can create single or multiple objects in TAD.

There are many ways to create an object. As indicated elsewhere in this documentation, an object need not be something you can touch and feel (i.e. some built-matter) In TAD, one is able to work with spaces too. In fact, one can even insert _pseudo-objects_ or objects that have no architectural meaning but are mere place holders (e.g. the viewpoint from where to look at the 3D scene, light locations, etc)

Objects may be 2D or 3D.

However; one always first creates a shape in _plan_ on some reference plane (often the ground itself) and then extrude that shape later to get the **3D volume** you want. In TAD 2D and 3D shapes co-exist. Of course, when you invoke the 3D Draft view command, only the 3D volumes would be visible.

Here is how one creates a new object:

1. In the **Class Pane**, select the class where you want to create an object.
2. On the **Create** menu, click **Create new object**. Alternately, you can press **Ctrl + Shift + F1**.
3. Some of the hotkeys that we have to [create objects are listed here](https://docs.teamtad.com/createhotkeys)

**Note**: Alternately, press **=** (equals to) followed by a name to create an object. The default size of this object is 1 unit x 1 unit.

**Shapes from the web**\
From version 6.7.7.0 onwards, TAD now has the capability to import all kinds of shapes from the system clipboard. Once you invoke the _creation_ floating dialog; you would see a largish _TAD Shapes_ button. Click on that, and the browser on your computer would open to a website where you can sketch out TAD shapes

In future; more such websites would crop up at multiple locations. You can list out those URLs in a text file called tadshapeurls.txt It is in the same folder where you installed the main executable of TAD. Simply add to that list, as you find more websites that can yield TAD Shapes. We have created one here [https://tad.in.net/goodies/tadsketcher0.5.html](https://tad.in.net/goodies/tadsketcher0.5.html)

The instructions for using that [TAD Sketcher](https://docs.teamtad.com/tadsketcher) is available. Other developers can make similar utilities and you can use them to create shapes and insert those shapes into TAD

**IMPORTANT difference between TAD and CAD**\
In CAD softwares; an architect would lovingly create the shape in the manner the architect wants; as he inserts that shape into the CAD environment. TAD does not work like that. TAD wants you to first create _some shape or the other_ so that you can quickly get to other aspects of your design. You can lovingly edit all shapes later on; to get it to be the way you wanted in your mind. This is a paradigm shift. TAD, initially seems more non-visual and conceptual. We believes it frees your mind and asks your mind to think about other _logic_ of your design; other than the visual.

The _Create_ menu will bring up a tabbed dialog; from where you can create the starting shapes for the objects in many different ways. Once you become an expert; you can also use the [Headsup Command Line](https://docs.teamtad.com/actshowcommandline) to directly create shapes.

* [Create an object](https://docs.teamtad.com/create\_an\_object)
* [Creating outlines](https://docs.teamtad.com/creating\_an\_outline)
* [Creating reflections](https://docs.teamtad.com/creating\_a\_reflection)
* [Merging shapes](https://docs.teamtad.com/actmerge)
* [Breaking an object](https://docs.teamtad.com/breaking\_an\_object)

```
... more (this page will be edited soon)
```

**Once you create an object, some of the common activities that are often done**\


1. In the **Site Info** pane, click the **Object** tab.
2. Enter height for the object.
3. Select a level for the object. The level refers to the level from the ground plane.
4. Right click **'isKind of'** to select an 'isKindOf' value. An object can be an atom, connector, envelope or an artefact. For more information on objects, see Types of objects in TAD. These concepts are described in detail in [kind of objects.](https://docs.teamtad.com/objects\_in\_tad)

Note that the object that you created is automatically added to the current class. If that is not what you expected; you can always drag the name of the object in the object list to the correct class.

[Advanced methods for setting attributes of an object](https://docs.teamtad.com/advanced\_methods\_for\_setting\_attributes\_of\_an\_object)

**See also:** [Create objects](https://docs.teamtad.com/actcreateobjnew) | [Headsup CommandLine](https://docs.teamtad.com/actshowcommandline) | [Rotate Precisely](https://docs.teamtad.com/action12) | [Free rotation](https://docs.teamtad.com/isrotating) | [Delete](https://docs.teamtad.com/action5) | [Free Dragging](https://docs.teamtad.com/isdraggingobj) | [Delete a corner](https://docs.teamtad.com/action18) | [Add a corner](https://docs.teamtad.com/action19) | [Shift a corner](https://docs.teamtad.com/action17) | [Undo](https://docs.teamtad.com/action15) | [Redo](https://docs.teamtad.com/action16) | [Precise move](https://docs.teamtad.com/action1) | [Stretch Side](https://docs.teamtad.com/action13) | [Extrude Side](https://docs.teamtad.com/action14) | [Edge Type](https://docs.teamtad.com/docurve) | [Step Size](https://docs.teamtad.com/stepsizeview) | [Advanced methods for setting attributes of an object](https://docs.teamtad.com/advanced\_methods\_for\_setting\_attributes\_of\_an\_object) | [Searching Objects and Classes](https://docs.teamtad.com/searchobjclass)

***

_Press F1 inside the application to read context-sensitive help directly in the application itself_\
_←_ [_∈_](https://docs.teamtad.com/create\_a\_new\_object?do=edit)
