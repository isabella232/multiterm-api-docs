

# 
    Load method



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Load —          Updates the selected layout from an external layout definition file.



## Returntype

void



## Parameters

* FileName (String)




## Description



By applying this method to a layout you can update the layout from the content of an external layout definition (\*.xdl) file.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout=oLayouts["My own layout"];
oLayout.Load("c:\\temp\\external_layout.xdl");
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Load)

