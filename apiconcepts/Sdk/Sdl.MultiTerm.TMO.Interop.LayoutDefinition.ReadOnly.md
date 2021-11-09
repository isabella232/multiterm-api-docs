

# 
    ReadOnly property



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.ReadOnly —          Returns whether a particular layout is read-only.



## Type

Boolean

(read)



## Index Parameters
*none*


## Description



Layouts may be read-only, e.g. when the termbase administrator provides a central layout, which is not supposed to be altered by the end users. Via this property you can ascertain whether a particular layout is read-only for the currently logged-in user.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout=oLayouts["Flags layout"];
Debug.WriteLine("Is layout read-only? " + oLayout.ReadOnly);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinition.ReadOnly)

