# Count property
## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinitions.Count —          Returns the number of available filter definitions.

## Type

Long
(read)


## Index Parameters
*none*

## Description

Via this property you can ascertain how many filter definitions are associated with a particular termbase.

## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

FilterDefinitions oFilters = oTb.FilterDefinitions;
Debug.Write("Number of filters: +" + oFilters.Count);
```
