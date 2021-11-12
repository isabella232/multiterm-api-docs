# Name property

## Name

Sdl.MultiTerm.TMO.Interop.LayoutDefinition.Name —          Returns the name of the layout.

## Type

String
(read)


## Index Parameters
*none*

## Description

Each layout has a unique descriptive name. This is the name that end users usually get to see in a MultiTerm client application. For example, this is the name that is listed in the layout dropdown list of MultiTerm Workstation.

Layouts can be referenced via this unique name.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select layout
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout;

//return list of layout names
for(int i=0;i<oLayouts.Count;i++)
{
   	oLayout = oLayouts[i];
   	Debug.WriteLine(oLayout.Name);
}
```
