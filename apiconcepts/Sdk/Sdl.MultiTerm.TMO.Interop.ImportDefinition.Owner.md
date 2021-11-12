#  Owner property

## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.Owner —          Returns the owner name for a particular import definition.

## Type

String
(read)

## Index Parameters
*none*

## Description

## Sample


```cs
Sdl.MultiTerm.TMO.Interop.ImportDefinitions oImportDefs = myTermbase.ImportDefinitions;
//return owner of first Import definition
Debug.WriteLine(oImportDefs[0].Owner);
```
