#  Name property

## Name

Sdl.MultiTerm.TMO.Interop.EntryField.Name —          Returns the name, i.e. the label of a particular entry-level descriptive field.


## Type
String
(read)

## Index Parameters
*none*

## Description


## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];

//select a particular entry
Entries oEntries = oTb.Entries;
Entry oEntry = oEntries.Item(1);
EntryContent content = oEntry.Content;
EntryFields oFields = content.Fields;
EntryField oField = oFields[0];
Debug.WriteLine("Field label: " + oField.Name);
```
