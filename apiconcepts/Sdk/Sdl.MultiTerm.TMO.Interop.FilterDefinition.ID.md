

# 
    ID property



## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.ID —          Returns the unique id of the filter.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Each filter is referenced in the database backend using a unique id, which the 'normal' user never gets to see. You can use this property to retrieve the corresponding id.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;
FilterDefinition oFilter = oFilters["Missing target"];

Debug.WriteLine(oFilter.ID);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinition.ID)

