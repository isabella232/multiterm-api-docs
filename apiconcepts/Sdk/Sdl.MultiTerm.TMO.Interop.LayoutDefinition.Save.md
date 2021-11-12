# Save method

## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Save —          Saves the layout definition to an external file.

## Returntype

void

## Parameters

* FileName (String)

## Description



Applying this method to a particular layout definition saves the content of the layout definition to an external file. Note that you need to provide the file path and name as well as the extension (\*.xdl) as parameter.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout=oLayouts["Flags layout"];
oLayout.Save("c:\\temp\\external_file");
```
