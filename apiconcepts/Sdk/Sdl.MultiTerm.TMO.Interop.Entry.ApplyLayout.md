#  ApplyLayout method

## Name

Sdl.MultiTerm.TMO.Interop.Entry.ApplyLayout —          Applies a layout definition to a MultiTerm entry XML stream.

## Returntype
String

## Parameters

* SourceIndex (String)
* TargetIndex (String).md)
* LayoutDefinitionObject ([Sdl.MultiTerm.TMO.Interop.LayoutDefinition](Sdl.MultiTerm.TMO.Interop.LayoutDefinition.md))


## Description

MultiTerm entries are stored in XML format, i.e. each entry can be output as an XML stream. For display purposes entries should be rendered in a more readable format, e.g. HTML.

Suppose you would like to display an entry in an HTML control. In this case you can apply a layout definition to the specified entry. Layout definitions contain an XSL stylesheet for rendering MultiTerm XML as HTML.

This method requires a layout definition object as parameter. A layout object can be selected either via the corresponding index number or via its unique termbase object name, which is case-sensitive, e.g. Layouts["Flags Layout"] or Layouts[0].

Additionally it also requires a source and target index, as layouts usually make use of source and target as logical fields.



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);

//select export definition
LayoutDefinitions oLayouts = oTb.LayoutDefinitions;
LayoutDefinition oLayout = oLayouts["Flags layout"];


string content = oEntry.ApplyLayout("English", "German", oLayout);
Debug.Write(content);
```
