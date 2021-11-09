

# 
    Active property



## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Active —          Activates a particular filter.



## Type

Boolean

(read / write)



## Index Parameters
*none*


## Description



This property can be used to activate (or deactivate) a filter. To activate a filter, set this property to true. The filter will then be applied to subsequent search operations. Via this property you can also ascertain whether a filter is active or not.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;
FilterDefinition oFilter = oFilters["Missing target"];

//activate filter
oFilter.Active = true;
Debug.WriteLine("Is filter active? " + oFilter.Active);

//deactivate filter
oFilter.Active = false;
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinition.Active)

