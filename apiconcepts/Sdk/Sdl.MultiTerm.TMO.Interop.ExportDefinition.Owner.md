#  Owner property

## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.Owner —          Returns the owner name for a particular export definition.

## Type
String
(read)

## Index Parameters
*none*

## Description



## Sample


```cs
Sdl.MultiTerm.TMO.Interop.ExportDefinitions oExportDefs = myTermbase.ExportDefinitions;
//return owner of first export definition
Debug.WriteLine(oExportDefs[0].Owner);
```

