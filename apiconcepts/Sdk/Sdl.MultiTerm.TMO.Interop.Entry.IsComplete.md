# IsComplete property

## Name

Sdl.MultiTerm.TMO.Interop.Entry.IsComplete —          Returns whether an entry is complete or not.

## Type

Boolean
(read)

## Index Parameters
*none*

## Description



An entry is considered incomplete if it lacks one or more fields that are mandatory according to the termbase definition. This property returns true if the current entry is complete, false if it is incomplete.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);
Debug.Write("Is entry complete? " + oEntry.IsComplete);
```


