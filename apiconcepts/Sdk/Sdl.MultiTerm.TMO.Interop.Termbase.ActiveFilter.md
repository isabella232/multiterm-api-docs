

# 
    ActiveFilter property




## Name

Sdl.MultiTerm.TMO.Interop.Termbase.ActiveFilter —          Returns the active filter for a termbase.



## Type
.md)
[Sdl.MultiTerm.TMO.Interop.FilterDefinition](Sdl.MultiTerm.TMO.Interop.FilterDefinition.md)

(read)



## Index Parameters
*none*


## Description



A filter allows you to search a termbase for a specific subset of entries, e.g. all entries that were created after a specified date. Filters are useful for search, import and export operations. If no filter is applied, a search or import/export operation will apply to all entries of a termbase. If a filter is used only entries that correspond to the filter will be processed.



## Sample


```cs
Termbase oTb = oTbs["Termbase Name"];

FilterDefinitions oFilters = oTb.FilterDefinitions;
FilterDefinition oFilter = oFilters["Missing target"];
oFilter.Active=true;
Debug.Write("Currently active filter: " + oTb.ActiveFilter.Name);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.Termbase.ActiveFilter)

