

# 
    Sdl.MultiTerm.TMO.Interop.ExportDefinition class



## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition —          Provides programmatic access to a particular export definition.



## Description



Export definitions contain an XSL stylesheet that transforms MultiTerm XML into the specified export format, e.g. TXT, HTML, RTF, etc. Via this class you can retrieve information on a particular export definition, e.g. the export definition description, the content (i.e. the export definition 'source code'), etc. In addition you can also use this class to edit an existing export definition with the export definition wizard.



## Properties

* [Content](Sdl.MultiTerm.TMO.Interop.ExportDefinition.Content.html): Returns the export definition content.
* [Description](Sdl.MultiTerm.TMO.Interop.ExportDefinition.Description.html): Returns the export definition description.
* [Name](Sdl.MultiTerm.TMO.Interop.ExportDefinition.Name.html): Returns the name of the export definition.
* [Owner](Sdl.MultiTerm.TMO.Interop.ExportDefinition.Owner.html): Returns the owner name for a particular export definition.
* [ReadOnly](Sdl.MultiTerm.TMO.Interop.ExportDefinition.ReadOnly.html): Returns whether a particular export definition is read-only.




## Methods

* [Delete](Sdl.MultiTerm.TMO.Interop.ExportDefinition.Delete.html): Removes the export definition from the collection.
* [Load](Sdl.MultiTerm.TMO.Interop.ExportDefinition.Load.html): Updates the selected export definition from an external export definition file.
* [ProcessExport](Sdl.MultiTerm.TMO.Interop.ExportDefinition.ProcessExport.html): Carries out the actual export process.
* [Save](Sdl.MultiTerm.TMO.Interop.ExportDefinition.Save.html): Saves the export definition to an external file.
* [StartWizard](Sdl.MultiTerm.TMO.Interop.ExportDefinition.StartWizard.html): Calls up the export wizard for editing a particular export definition.




## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
Debug.WriteLine(oExpDef.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ExportDefinition)

