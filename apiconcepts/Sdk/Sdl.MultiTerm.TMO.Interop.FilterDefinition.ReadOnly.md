# ReadOnly property

## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.ReadOnly —          Returns whether a particular filter is read-only.

## Type

Boolean
(read)

## Index Parameters
*none*

## Description

Filters may be read-only, e.g. when the termbase administrator provides a central filter, which is not supposed to be altered by the end users. Via this property you can ascertain whether a particular filter is read-only for the currently logged-in user.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;

FilterDefinition oFilter = oFilters["Missing target"];
Debug.WriteLine("Filter is read-only? " + oFilter.ReadOnly);
```