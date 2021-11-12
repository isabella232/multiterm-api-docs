# Owner property

## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Owner —          Returns the owner name for a particular filter definition.

## Type

String
(read)

## Index Parameters
*none*

## Description


## Sample


```cs
Sdl.MultiTerm.TMO.Interop.FilterDefinitions oFilters = myTermbase.FilterDefinitions;
//return owner of first filter definition
Debug.WriteLine(oFilters[0].Owner);
```
