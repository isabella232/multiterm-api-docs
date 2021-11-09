

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Count —          Returns the number of available input model definitions.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain how many input model definitions are associated with a particular termbase.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

InputModelDefinitions oModels = oTb.InputModelDefinitions;
Debug.Write("Number of input models: +" + oModels.Count);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinitions.Count)

