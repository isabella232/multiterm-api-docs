

# 
    Description property



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.Description —          Returns the import definition description.



## Type

String

(read)



## Index Parameters
*none*


## Description



Each import definition can have an optional description to provide further information on it. Via this property you can output the import definition description string.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs["Default import definition"];
Debug.Write(oImpDef.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.Description)

