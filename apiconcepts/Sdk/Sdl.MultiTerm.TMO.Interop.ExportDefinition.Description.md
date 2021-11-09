

# 
    Description property



## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.Description —          Returns the export definition description.



## Type

String

(read)



## Index Parameters
*none*


## Description



Each export definition can have an optional description to provide further information on it. Via this property you can output the export definition description string.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
Debug.WriteLine(oExpDef.Description);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ExportDefinition.Description)

