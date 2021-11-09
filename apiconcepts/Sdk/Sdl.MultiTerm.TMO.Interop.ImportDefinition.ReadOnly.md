

# 
    ReadOnly property



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.ReadOnly —          Returns whether a particular import definition is read-only.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



Import definitions may be read-only, e.g. when the termbase administrator provides a central import definition, which is not supposed to be altered by the end users. Via this property you can ascertain whether a particular import definition is read-only for the currently logged-in user.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs["Default import definition"];
Debug.WriteLine("Is this import definition read-only for me? " + oImpDef.ReadOnly);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.ReadOnly)

