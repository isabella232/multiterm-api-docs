#  ID property

## Name

Sdl.MultiTerm.TMO.Interop.Entry.ID —          Returns the id of an entry.

## Type
Long
(read)

## Index Parameters
*none*

## Description

Each termbase entry can be referenced via its unique entry id. This property returns the id of a particular entry.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);
Debug.Write("Current entry id: " + oEntry.ID);
```

