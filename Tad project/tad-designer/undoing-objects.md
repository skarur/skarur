# Undoing objects

Summary:

1. In the **Class Pane**, select the object that you want to undo a recent action.
2. In the **Edit** menu, click **Undo**. Alternately, you can press **Ctrl + Alt + Z**.

You can undo 10 commands per object.

**Details:**

The _Undo_ editing action is very powerful. TAD has a very unique way of preserving undo history — practically no other software has this method. so please read this topic carefully. _It will make you a lot more efficient._

EACH object inside TAD keeps its own undo history; and therefore you can do _out-of-turn undos_

Let me explain: Say you have 3 objects: A, B, and C and you made changes as follows, in the following sequence:

A was moved\
B was rotated\
C was edited

That means, C was the last object you edited (and the helpers would now be located on C) Now if you shift the helpers back to object B … that means, now B is the current object

Now you invoke this _undo_ action; and viola you would find that ONLY B returns back to its previous state. TAD will neither take A and nor C to its earlier form

This saves a huge lot of time; because you can cherry pick the objects you want to carry out an undo on. This action is also intelligent enough to work similarly when you invoke this action on multiple (i.e. selected) objects

**One more powerful feature of the **_**undo**_** action, is that undos are preserved across editing sessions! That means, when you save a file; the undo history is preserved on your drive; and when you load the same file back again later; you will find that you can still undo the objects as before!!**

_NOTE: Each object does not have infinite undo capabilities! Each object preserves around 10 undo states_

_**NOTE ALSO:** Creation and deletion of objects cannot be undone! However, when you delete any object/s they go into the_ [Recycle Bin](https://docs.teamtad.com/recycle\_bin) _and you can undelete it from there_

**See also:** [Create objects](https://docs.teamtad.com/actcreateobjnew) | [Headsup CommandLine](https://docs.teamtad.com/actshowcommandline) | [Rotate Precisely](https://docs.teamtad.com/action12) | [Free rotation](https://docs.teamtad.com/isrotating) | [Delete](https://docs.teamtad.com/action5) | [Free Dragging](https://docs.teamtad.com/isdraggingobj) | [Delete a corner](https://docs.teamtad.com/action18) | [Add a corner](https://docs.teamtad.com/action19) | [Shift a corner](https://docs.teamtad.com/action17) | [Undo](https://docs.teamtad.com/undo\_objects#plugin\_include\_\_action15) | [Redo](https://docs.teamtad.com/action16) | [Precise move](https://docs.teamtad.com/action1) | [Stretch Side](https://docs.teamtad.com/action13) | [Extrude Side](https://docs.teamtad.com/action14) | [Edge Type](https://docs.teamtad.com/docurve) | [Step Size](https://docs.teamtad.com/stepsizeview) | [Advanced methods for setting attributes of an object](https://docs.teamtad.com/advanced\_methods\_for\_setting\_attributes\_of\_an\_object) | [Searching Objects and Classes](https://docs.teamtad.com/searchobjclass)

***

_Press F1 inside the application to read context-sensitive help directly in the application itself_\
_←_ [_∈_](https://docs.teamtad.com/undo\_objects?do=edit)
