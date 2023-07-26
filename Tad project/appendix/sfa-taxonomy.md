# SFA Taxonomy

Taxonomy means a classification system. SFA stands for **Sabu Francis and Associates**, the architectural practice which discovered and used this taxonomy in all their projects.

The SFA Taxonomy is based on the fractal theories in geometry. According to the fractal theory, all the volumes in architecture designs can be represented by either solids or spaces.

In TAD, objects are classified in the following types:

* **Atom** - It represents a space that is not further sub-divided in the minds-eye of the architect. For example; when designing a building, an _atom_ would be the rooms in the building. But this actually depends on the scale of the design. If you are designing a table; it would be possible the architect considers the space below the material of the table, where your legs would go into; that space could be an atom for that scale of design. And so on, for other scales.
* **Envelope** - It represents an enclosure space that _wraps_ other spatial elements.
* **Connector** - It represents spatial elements that connects between other spatial elements. For example, Doors and windows. [Read more on how one works with connectors here](https://docs.teamtad.com/working\_with\_connectors)
* **Artefacts** - It represents elements that cannot be further sub-divided at the current level of investigation. For example, canopies, interior furniture, and other similar objects. Think of _artefacts_ as either fully solid matter For eg - Chajjas (aka sunshades), canopies etc… or they are to be later broken down further into its constituent ''atoms“, “envelopes” and “connectors ”; when the design gets detailed out.
* **Linked-nodes** - It represents a set of artefacts that are linked to each other. For example, column-beam frame.
* **Pseudo objects** - It represents the objects that are not actual built objects. For example, referential objects like lights, location, and look at.

You may wonder where the _walls_ are represented here. Well, by and large; walls are a _bye-product_ of the fact that we classify spaces into atoms, envelopes and connectors. When you place spatial objects as per the aforesaid taxonomy, the 3D CSG (boolean) operations of subtracting the atoms and connectors from the envelopes would yield the _walls_

Of course, I am referring here to the scale of a building here. What I should have mentioned is that the boolean operation yields the _left-over_ (that is the correct technical term we use) which stand for the built-matter after the boolean operation is done. So to give an example at another scale; say you are designing a table; then this boolean operation would yield the amount of _wood_ i.e. the material that would go to make the table.

You may have guessed that in TAD we largely _invert_ the CAD process. In CAD one largely talks of the edges of solid matter. But in TAD we often represent spaces; and the solid matter _emerges_ as a bye-product of having placed the spatial elements of atoms, connectors into envelopes.

**Note**: In TAD, objects are assigned their category in this taxonomy via **isKindOf** option in [the Site Info Pane](https://docs.teamtad.com/the\_site\_info\_pane).

***

_Press F1 inside the application to read context-sensitive help directly in the application itself_\
_←_ [_∈_](https://docs.teamtad.com/sfa\_taxonomy?do=edit)\
