

# 
    Description property



## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Description —          Returns the filter description.



## Type

String

(read)



## Index Parameters
*none*


## Description



Each filter can have an optional description to provide further information on it. Via this property you can output the filter description string.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;
FilterDefinition oFilter = oFilters["Missing target"];

Debug.WriteLine("Filter description: " + oFilter.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinition.Description)

