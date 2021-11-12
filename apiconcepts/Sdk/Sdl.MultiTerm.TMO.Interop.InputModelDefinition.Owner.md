#  Owner property

## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Owner —          Returns the owner name for a particular input model definition.

## Type

String
(read)

## Index Parameters
*none*


## Description


## Sample


```cs
Sdl.MultiTerm.TMO.Interop.InputModelDefinitions oInputModels = myTermbase.InputModelDefinitions;
//return owner of first Layout definition
Debug.WriteLine(oInputModels[0].Owner);
```
