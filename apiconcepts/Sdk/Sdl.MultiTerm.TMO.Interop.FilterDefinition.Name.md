

# 
    Name property



## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Name —          Returns the name of the filter.



## Type

String

(read)



## Index Parameters
*none*


## Description



Each filter has a unique descriptive name. This is the name that end users usually get to see in a MultiTerm client application. For example, this is the name that is listed in the filter dropdown list of MultiTerm Workstation.

Filters can be referenced via this unique name.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;

FilterDefinition oFilter;
for(int i=0;i<oFilters.Count;i++)
{
   	oFilter = oFilters[i];
   	Debug.WriteLine(oFilter.Name);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinition.Name)

