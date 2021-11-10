

# 
    Sdl.MultiTerm.TMO.Interop.InputModelDefinition class




## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition —          Provides access to a particular input model definition.



## Description



Input models are customizable input masks that facilitate the process of adding or editing entries via, e.g. MultiTerm Workstation or MultiTerm Online. Using this class you can retrieve information on a particular input model, e.g. the input model description string. In addition you can use this class to load an input model, save it to an external file, etc.



## Properties
.md)
* [Content](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Content.md): Returns the content of a particular input model definition.
* [Description](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Description.md): Returns the input model definition description.
* [Name](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Name.md): Returns the name of the input model definition.
* [Owner](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Owner.md): Returns the owner name for a particular input model definition.
* [ReadOnly](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.ReadOnly.md): Returns whether a particular input model definition is read-only.




## Methods

* [\_GetSchema](Sdl.MultiTerm.TMO.Interop.InputModelDefinition._GetSchema.md): Returns the full schema for a particular input model.
* [Delete](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Delete.md): Removes the input model definition from the collection.
* [GetDummyEntry](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.GetDummyEntry.md): [For internal use only.]
* [Load](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Load.md): Updates the selected input model from an external input model definition file.
* [Save](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Save.md): Saves the input model definition to an external file.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.InputModelDefinition.StartWizard.md): Calls up the input model wizard for editing a particular input model.




## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["Default input model"];
Debug.WriteLine(oInputModel.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinition)

