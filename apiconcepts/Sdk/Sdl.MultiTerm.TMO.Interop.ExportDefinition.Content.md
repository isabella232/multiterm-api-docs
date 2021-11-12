# Content property

## Name
Sdl.MultiTerm.TMO.Interop.ExportDefinition.Content —          Returns the export definition content.

## Type
String
(read)

## Index Parameters
*none*

## Description

An export definition contains an XSL stylesheet, which is used to render MultiTerm XML entry content into the requested export format, e.g. TXT, HTML, RTF, etc. Via this property you can output the content, i.e. the 'source code' of the export definition.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select an export definition
ExportDefinitions oExpDefs = oTb.ExportDefinitions;
ExportDefinition oExpDef = oExpDefs["Default export definition"];
Debug.WriteLine(oExpDef.Content);
```


