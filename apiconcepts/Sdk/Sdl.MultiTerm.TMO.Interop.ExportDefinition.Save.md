

# 
    Save method



## Name

Sdl.MultiTerm.TMO.Interop.ExportDefinition.Save —          Saves the export definition to an external file.



## Returntype

void



## Parameters

* FileName (String)




## Description



Applying this method to a particular export definition saves the content of the export definition to an external file. Note that you need to provide the file path and name as well as the extension (\*.xdx) as parameter.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
oExpDef.Save("c:\\temp\\export.xdx");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.ExportDefinition.Save)

