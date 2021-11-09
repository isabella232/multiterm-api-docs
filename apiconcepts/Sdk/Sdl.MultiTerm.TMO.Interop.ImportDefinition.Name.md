

# 
    Name property



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinition.Name —          Returns the name of the import definition.



## Type

String

(read)



## Index Parameters
*none*


## Description



Each import definition has a unique descriptive name. For example, this is the name that is listed in the import definition list of the Termbase Catalogue in MultiTerm Workstation.

All import definitions can be referenced via this unique name.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select import definition
ImportDefinitions oExpDefs = oTb.ImportDefinitions;
ImportDefinition oExpDef;

//return list of import definition names
for(int i=0;i<oImpDefs.Count;i++)
{
   oImpDef = oImpDefs[i];
   Debug.WriteLine(oImpDef.Name);
}
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinition.Name)

