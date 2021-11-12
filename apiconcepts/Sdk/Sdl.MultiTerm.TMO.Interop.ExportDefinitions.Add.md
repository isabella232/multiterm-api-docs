# Add method




## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinitions.Add —          Adds a new export definition to the collection.



## Returntype
[Sdl.MultiTerm.TMO.Interop.ExportDefinition](Sdl.MultiTerm.TMO.Interop.ExportDefinition.md)



## Parameters

* Name (String)
* Description (String)
* FileName (String)




## Description



Applying this method to an export definition collection adds a new export definition from an export definition that was saved as an external \*.xdx file. This method requires the name of the new export definition, an optional description and the full path and name of the export definition file.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oExpDefs = oTb.ExportDefinitions;
oExpDefs.Add("Export definition name", "Export definition description", "c:\\temp\\exp_def.xdx");
```

