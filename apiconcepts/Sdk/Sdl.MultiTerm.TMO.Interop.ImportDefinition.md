

# 
    Sdl.MultiTerm.TMO.Interop.ImportDefinition class



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition —          Provides programmatic access to a particular import definition.



## Description



Import definitions are used to import the content from MultiTerm XML files into a termbase. Via this class you can retrieve information on a particular import definition, e.g. the description string or programmatically trigger the import process.



## Properties

* [Content](Sdl.MultiTerm.TMO.Interop.ImportDefinition.Content.html): Returns the content of a particular import definition in an XML format.
* [Description](Sdl.MultiTerm.TMO.Interop.ImportDefinition.Description.html): Returns the import definition description.
* [Name](Sdl.MultiTerm.TMO.Interop.ImportDefinition.Name.html): Returns the name of the import definition.
* [Owner](Sdl.MultiTerm.TMO.Interop.ImportDefinition.Owner.html): Returns the owner name for a particular import definition.
* [ReadOnly](Sdl.MultiTerm.TMO.Interop.ImportDefinition.ReadOnly.html): Returns whether a particular import definition is read-only.




## Methods

* [Delete](Sdl.MultiTerm.TMO.Interop.ImportDefinition.Delete.html): Removes the import definition from the collection.
* [Load](Sdl.MultiTerm.TMO.Interop.ImportDefinition.Load.html): Updates the selected import definition from an external import definition file.
* [ProcessImport](Sdl.MultiTerm.TMO.Interop.ImportDefinition.ProcessImport.html): Carries out the actual import process.
* [Save](Sdl.MultiTerm.TMO.Interop.ImportDefinition.Save.html): Saves the import definition to an external file.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.ImportDefinition.StartWizard.html): Calls up the import wizard for editing a particular import definition.




## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs["Default import definition"];
Debug.Write(oImpDef.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition)

