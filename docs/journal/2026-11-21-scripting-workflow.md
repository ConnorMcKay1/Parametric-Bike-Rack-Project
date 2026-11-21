# 2026-11-21-scripting-workflow.md

## A bit of programming

As I work towards the end stages of assembly of the bike rack in FreeCAD I have been paying more attention to the underlying Python used to perform each action.
And since there is a Python terminal embedded in the GUI I figured there must be some sort of workflow; scripting users are what the developers of FreeCAD call a "Super User".

Even though FreeCAD has a built in Terminal, it is not great from a UX perspective. So to fix this all the coding is done in an external IDE (VScode in my case).

To make this easier this easier, it is recommended to access the documentation API (not the runtime functions though, just the "stub") to allow for auto complete
and other 'intellisense' features.

The FreeCAD stub was from PyPI (Python Package Index) into my Global environment manager in VScode

The Pylance extension automatically picks up on the documentation source so that when the FreeCAD package is imported, such as:
  import FreeCAD as App
  import FreeCAD as Gui
  import FreeCAD as Part
  import FreeCAD as Mesh
a list of attributes/functions is displayed when ever the typical "." is used after an object with properties, such as:
  App.ActiveDocument
  doc.getObject()
    --and geometry based actions:
  shape = obj.Shape
    print(shape.Volume)

Even though I can now write Python scripts for FreeCAD in an IDE I still have to execute them in FreeCAD.
This isn't too tedious as these scripts do not have to be copy/pasted and can simply be imported into FreeCAD's execution environment by
using the Python terminal to open the scripting file and be executed from there.


This workflow is quite nice and although it cannot do certain tasks, such as execution inside IDE, it will definitely aid in me learning how to be more efficient
and automate geometry creation and simulations.














    
