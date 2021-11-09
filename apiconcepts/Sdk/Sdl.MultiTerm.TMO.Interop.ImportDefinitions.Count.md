

# 
    Count property



## Name

Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Count —          Returns the number of available import definitions.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Via this property you can ascertain how many import definitions are associated with a particular termbase.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

ExportDefinitions oImpDefs = oTb.ImportDefinitions;
Debug.Write("Number of import definitions: +" + oImpDefs.Count);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ImportDefinitions.Count)

