

# 
    Delete method



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.Delete —          Removes the import definition from the collection.



## Returntype

void



## Parameters
*none*


## Description



Applying this method removes the import definition physically from the collection of import definitions. This can only be done, if the currently logged-in user is allowed to delete the import definition in question. If the user does not have the right to delete the import definition, a corresponding error message will be thrown. Users usually can only delete import definitions created by themselves.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an import definition
ImportDefinitions oImpDefs = oTb.ImportDefinitions;
ImportDefinition oImpDef = oImpDefs["Default import definition"];
oImpDef.Delete();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.Delete)

