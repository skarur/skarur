# Exporting objects to 3D

To export as a 3D file,

1. In the **File** menu, select **Export to various 3D formats**
2. In the **Export as a VRML 2 file** box, select the file type you want to export as.
3. Assign a name to the file and click **Save**

Note:

When you export to VRML 2.0, the camera is set as per the location and lookat objects. Moreover, it is possible to incorporate VRML materials directly into TAD when exporting to VRML 2.0.

In order to get materials in the exported VRML file, first you should understand the syntax of a special materials file used by TAD

This file is called tad.mat and it should be kept in a sub-directory “materials” of the TAD file which is being processed. Alternatively, if such a file is not present the TAD would attempt to load tad.mat from TAD's system folder (folder where the TAD executable and this help file is kept). The second option is better, if the office using TAD has a uniform system of materials used in all their projects.

tad.mat should have lines of the following type

m(MaterialNameStr,ListOfMaterialProperties)

The ListOfMaterialProperties should be within square brackets and it should contain the following (all are optional, non-repetitive):

transparency(number) specularColor(number,number,number) shininess(number) emissiveColor(number,number,number) diffuseColor(number,number,number) ambientIntensity(number) imageTexture(string) textureScale( number,number)

In the above, all properties dealing with Color (e.g. emmisiveColor(…)) takes three numeric values: First one is for Red, second is for Green and third is for Blue. The imageTexture(…) is a filename (JPG or GIF or PNG) which forms the texture of the surface being rendered. textureScale(…) tells how the imageTexture gets scaled in the x and y direction on the surface.

You can edit the tad.mat file which is present in the system folder of TAD, from within the Settings dialog (File | Settings)

An example of tad.mat is as follows:

![m(](https://docs.teamtad.com/lib/images/smileys/facepalm.svg)“transp”,\[transparency(0.5)]) ![m(](https://docs.teamtad.com/lib/images/smileys/facepalm.svg)“atom”,\[diffusecolor(0,0,0.9),shininess(0.8)]) ![m(](https://docs.teamtad.com/lib/images/smileys/facepalm.svg)“marble”,\[imagetexture(“marble.jpg”),shininess(0.8)]) ![m(](https://docs.teamtad.com/lib/images/smileys/facepalm.svg)“stucco”,\[vlf(“shader.shd”)])

You may wonder where the vlf(…) properties came from. Well that is meant for export to VirtuaLight and not for VRML. You will read about it when we examine export to VirtuaLight.

Okay, now the materials are defined. What next?

In order to place the materials on an object in the exported VRML 2 file, that object should be enriched with the following attribute “vrmlmtl(…)” For e.g. If we want to use the marble material on an object when it gets exported to VRML 2; then do the following:

Go to its class; right click for the menu, select Edit Ardela and give the following attribute in the inheritable portion of the Ardela editing dialog. Then confirm the editing and close it.

vrmlmtl(@,“marble”):-!.

All objects of that class (and sub-classes underneath it) will now be dressed up with marble. If you do not want that behavior, instead of placing vrmlmtl(…) in the object's class; you can go specifically to the object itself and give it in the “Self code” of its Ardela. (Right click on the object name in the Classes and Objects pane and select Edit Ardela)

Make sure that you use that material which was specifically meant for VRML 2. If you use the default tad.mat file, you cannot use “stucco” as a material name because that was meant for export to Virtualight and not VRML 2

B) Export to Virtualight You can setup tad.mat with two material properties that is specifically meant for VirtuaLight in the tad.mat file. One is vlf(…) and the other is vl(…)

vlf(filename) specifies an external filename which contains all the shading instructions that VirtuaLight recognizes. Consult VirtuaLight documentation for that. Specify the filename properly. If it contains backslashes, ensure that they are doubled-up. For e.g. if you want to refer to a file c:\a\b\c.txt then it would be specified as:

![m(](https://docs.teamtad.com/lib/images/smileys/facepalm.svg)“stucko”,\[vlf(“c:\\\a\\\b\\\c.txt”)])

If you use vl(string), then the shading instructions are placed directly within vl(…) (put within quotation marks)

In order to place the materials on an object in the exported Virtualight file, do the same as what was done for VRML except that the Ardela attribute to be added is

vlmtl(@,“materialname”):-!.

(substitute materialname with whatever that was defined for the Virtualight materials in tad.mat file)

C) Export to Renderman Renderman has only one material property that can be placed in the tad.mat file. That is rmf(…)

rmf(filename)

Its behaviour is same as that of vlf(…) for Virtualight.

In order to place the materials on an object in the exported Renderman file, do the same as what was done for VRML except that the Ardela attribute to be added is

rmmtl(@,“materialname”):-!.

(substitute materialname with whatever that was defined for the Renderman materials in tad.mat file)

***

_Press F1 inside the application to read context-sensitive help directly in the application itself_\
_←_ [_∈_](https://docs.teamtad.com/exporting\_objects\_to\_3d?do=edit)\
