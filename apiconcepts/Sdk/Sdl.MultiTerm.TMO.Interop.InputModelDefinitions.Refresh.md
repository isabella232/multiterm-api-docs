

# 
    Refresh method



## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Refresh —          Updates the input model definition collection.



## Returntype

void



## Parameters
*none*


## Description



By applying this method you can make sure that MultiTerm client users always have access to the up-to-date export definition collection, which includes all definitions that have been added while the users were online.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

InputModelDefinitions oModels = oTb.InputModelDefinitions;
oModels.Refresh();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Refresh)

