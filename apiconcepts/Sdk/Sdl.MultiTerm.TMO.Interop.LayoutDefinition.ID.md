

# 
    ID property



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.ID —          Returns the unique id of the layout.



## Type

Long

(read)



## Index Parameters
*none*


## Description



Each layout is referenced in the database backend using a unique id, which the 'normal' user never gets to see. You can use this property to retrieve the corresponding id.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout = oLayouts["Flags layout"];

Debug.WriteLine(oLayout.ID);
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinition.ID)

