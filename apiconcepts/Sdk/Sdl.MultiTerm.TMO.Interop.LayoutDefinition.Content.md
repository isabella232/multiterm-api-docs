# Content property

## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Content —          Returns the layout definition content.

## Type

String
(read)


## Index Parameters
*none*

## Description


A layout contains an XSL stylesheet, which is used to render MultiTerm XML entry content as HTML. Via this property you can output the content, i.e. the 'source code' of the layout definition.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout = oLayouts["Flags layout"];

Debug.WriteLine(oLayout.Content);
```
