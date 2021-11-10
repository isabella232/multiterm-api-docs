

# 
    Add method




## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinitions.Add —          Adds a new filter definition to the collection.



## Returntype
.md)
[Sdl.MultiTerm.TMO.Interop.FilterDefinition](Sdl.MultiTerm.TMO.Interop.FilterDefinition.md)



## Parameters

* Name (String)
* Description (String)
* FileName (String)




## Description



Applying this method to a filter definition collection adds a new filter definition from a filter definition that was saved as an external \*.xdf file. This method requires the name of the new filter definition, an optional description and the full path and name of the filter definition file.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

FilterDefinitions oFilters = oTb.FilterDefinitions;
oFilters.Add("Filter definition name", "Filter definition description", "c:\\temp\\missing_target_.xdf");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinitions.Add)

