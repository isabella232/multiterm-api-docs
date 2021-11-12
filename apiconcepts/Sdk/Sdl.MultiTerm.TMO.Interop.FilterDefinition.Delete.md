# Delete method

## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Delete —          Removes the filter from the collection.

## Returntype

void

## Parameters
*none*

## Description

Applying this method removes the filter physically from the collection of filter definitions. This can only be done, if the currently logged-in user is allowed to delete the filter in question. If the user does not have the right to delete the filter, a corresponding error message will be thrown.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;

FilterDefinition oFilter = oFilters["Missing target"];
oFilter.Delete();
```
