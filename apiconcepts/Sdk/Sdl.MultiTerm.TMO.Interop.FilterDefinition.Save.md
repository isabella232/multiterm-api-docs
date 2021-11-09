

# 
    Save method



## Name

Sdl.MultiTerm.TMO.Interop.FilterDefinition.Save —           Saves the filter definition to an external file.



## Returntype

void



## Parameters

* FileName (String)




## Description



Applying this method to a particular filter definition saves the content of the filter definition to an external file. Note that you need to provide the file path and name as well as the extension (\*.xdf) as parameter.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select filter
FilterDefinitions oFilters = oTb.FilterDefinitions;

FilterDefinition oFilter = oFilters["Missing target"];
oFilter.Save("c:\\temp\\filter.xdf");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.FilterDefinition.Save)

