# Description property

## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Description —          Returns the layout description.

## Type

String
(read)

## Index Parameters
*none*


## Description

Each layout can have an optional description to provide further information on it. Via this property you can output the layout description string.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout = oLayouts["Flags layout"];

Debug.WriteLine(oLayout.Description);
```

