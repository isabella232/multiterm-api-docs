

# 
    Content property



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.Content —          Returns the content of a particular import definition.



## Type

String

(read)



## Index Parameters
*none*


## Description



Via this property you can retrieve the 'source code' of an import definition.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs["Default import definition"];
Debug.Write(oImpDef.Content);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.Content)

