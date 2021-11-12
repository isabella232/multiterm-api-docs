# FilterDefinitions property

## Name

Sdl.MultiTerm.TMO.Interop.Termbase.FilterDefinitions —          Provides programmatic access to the filter definitions of a termbase.

## Type
[Sdl.MultiTerm.TMO.Interop.FilterDefinitions](Sdl.MultiTerm.TMO.Interop.FilterDefinitions.md)
(read)

## Index Parameters
*none*

## Description

Filters are used to search for a specific subset of entries that match a specified criteria (e.g. all entries that were created after a certain date, that contain or do not contain a particular field, etc.). After creation, each termbase is automatically assigned one default filter. Users can add further filters as required. The filter definitions are physically stored in in the termbase.

Via this property you can, for example, return the number of available filter definitions, generate a list containing the names of available filters, etc.

## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

FilterDefinitions oFilterDefs = oTb.FilterDefinitions;

Debug.Write("Total number of filter definitions in termbase: " + oFilterDefs.Count.ToString());
```

