

# 
    Content property



## Name

Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Content —          Returns the content of a particular input model definition.



## Type

String

(read)



## Index Parameters
*none*


## Description



Via this property you can retrieve the 'source code' of an input model definition.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select input model
InputModelDefinitions oInputModels = oTb.InputModelDefinitions;
InputModelDefinition oInputModel = oInputModels["Default input model"];
Debug.WriteLine(oInputModel.Content);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.InputModelDefinition.Content)

