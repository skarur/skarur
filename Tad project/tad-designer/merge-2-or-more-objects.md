# Merge 2 or more objects

This is a powerful command that creates an object by combining shape data from the current selection set. For this command to work, you MUST have two or more shapes in the selection set. Also, these shapes must overlap with each other.

The combined shape that is created is dependent on the way the shape was rendered inside TAD. You see, TAD shapes can either be _clockwise_ or _anti-clockwise_ As far as you are concerned, it does not matter – because visually it does not make any difference.

To know if a shape is clockwise or anti-clockwise; make that object the [current object](https://docs.teamtad.com/current\_object) and then press F3 repeatedly. If the red square dot (i.e. the first helper) is going clockwise, then you know that the shape is drawn clockwise!

When you use this command TAD cleverly _merges together_ (in graphic theory it is called a _union_) all the clockwise drawn shapes. If there are _anti-_clockwise shapes, then TAD will use that shape to cut out (like a stencil) from the other shapes.

The merge command is very useful to create [envelopes](https://docs.teamtad.com/envelope)

**See also:** [Create objects](https://docs.teamtad.com/actcreateobjnew) | [Headsup CommandLine](https://docs.teamtad.com/actshowcommandline) | [Rotate Precisely](https://docs.teamtad.com/action12) | [Free rotation](https://docs.teamtad.com/isrotating) | [Delete](https://docs.teamtad.com/action5) | [Free Dragging](https://docs.teamtad.com/isdraggingobj) | [Delete a corner](https://docs.teamtad.com/action18) | [Add a corner](https://docs.teamtad.com/action19) | [Shift a corner](https://docs.teamtad.com/action17) | [Undo](https://docs.teamtad.com/action15) | [Redo](https://docs.teamtad.com/action16) | [Precise move](https://docs.teamtad.com/action1) | [Stretch Side](https://docs.teamtad.com/action13) | [Extrude Side](https://docs.teamtad.com/action14) | [Edge Type](https://docs.teamtad.com/docurve) | [Step Size](https://docs.teamtad.com/stepsizeview) | [Advanced methods for setting attributes of an object](https://docs.teamtad.com/advanced\_methods\_for\_setting\_attributes\_of\_an\_object) | [Searching Objects and Classes](https://docs.teamtad.com/searchobjclass)

***

_Press F1 inside the application to read context-sensitive help directly in the application itself_\
_←_ [_∈_](https://docs.teamtad.com/merging\_objects?do=edit)
