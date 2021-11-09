

# 
    Delete method



## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Delete —          Removes the layout from the collection.



## Returntype

void



## Parameters
*none*


## Description



Applying this method removes the layout physically from the collection of layout definitions. This can only be done, if the currently logged-in user is allowed to delete the layout in question. If the user does not have the right to delete the layout, a corresponding error message will be thrown. Users usually can only delete layouts created by themselves.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout=oLayouts["My own layout"];
oLayout.Delete();
```



## Provide Feedback

[Make annotation](mailto:sdk-feedback@sdl.com&amp;subject=Reference%20for%20Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Delete)

