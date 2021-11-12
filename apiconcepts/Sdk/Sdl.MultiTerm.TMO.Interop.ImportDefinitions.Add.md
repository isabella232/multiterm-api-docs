# Add method

## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Add —          Adds a new import definition to the collection.

## Returntype
[Sdl.MultiTerm.TMO.Interop.ImportDefinition](Sdl.MultiTerm.TMO.Interop.ImportDefinition.md)



## Parameters

* Name (String)
* Description (String)
* FileName (String)


## Description

Applying this method to an export definition collection adds a new import definition from an import definition that was saved as an external \*.xdi file. This method requires the name of the new import definition, an optional description and the full path and name of the import definition file.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ImportDefinitions oImpDefs = oTb.Import definition description", "c:\\temp\\imp_def.xdi");
```

