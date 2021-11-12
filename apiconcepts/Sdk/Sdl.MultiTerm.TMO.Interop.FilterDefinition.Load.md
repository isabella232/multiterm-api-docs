# Load method

## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Load —          Updates the selected filter from an external filter definition file.

## Returntype

void

## Parameters

* FileName (String)

## Description

By applying this method to a layout you can update the filter from the content of an external filter definition (\*.xdf) file.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;

FilterDefinition oFilter = oFilters["Missing target"];
oFilter.Load("c:\\temp\\filter.xdf");
```