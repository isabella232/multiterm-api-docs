

# 
    Add method



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Add —          Adds a new layout definition to the collection.



## Returntype

[Sdl.MultiTerm.TMO.Interop.LayoutDefinition](Sdl.MultiTerm.TMO.Interop.LayoutDefinition.html)



## Parameters

* Name (String)
* Description (String)
* FileName (String)




## Description



Applying this method to an layout definition collection adds a new layout definition from a layout definition that was saved as an external \*.xdl file. This method requires the name of the new layout definition, an optional description and the full path and name of the layout definition file.



## Sample


```cs
Termbase oTb = oTbs["Termbase name"];

LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
oLayouts.Add("Layout definition name", "Layout definition description", "c:\\temp\\layout_def.xdl");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinitions.Add)

