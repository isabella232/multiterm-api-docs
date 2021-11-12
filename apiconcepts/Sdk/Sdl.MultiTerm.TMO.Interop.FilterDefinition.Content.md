#  Content property

## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Content —          Returns the filter definition content.

## Type

String
(read)

## Index Parameters
*none*

## Description

A filter contains an XPATH statement, which is applied to MultiTerm XML in order to ascertain whether the entry fits the statement or not. Via this property you can output the content, i.e. the 'source code' of the filter definition.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;
FilterDefinition oFilter = oFilters["Missing target"];

Debug.WriteLine(oFilter.Content);
```

