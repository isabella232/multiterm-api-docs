#  ReadOnly property

## Name

Sdl.MultiTerm.TMO.Interop.EntryField.ReadOnly —          Returns whether a particular entry-level descriptive field is read-only.

## Type
Boolean
(read)

## Index Parameters
*none*

## Description

Via this property you can ascertain whether a descriptive field is read-only for the currently logged-in user. It returns true, if it is read-only, otherwise false.

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
Debug.WriteLine("Field is read-only for me? " + oField.ReadOnly);
```
