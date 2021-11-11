# Delete method

## Name

Sdl.MultiTerm.TMO.Interop.Entry.Delete —          Removes an entry from the termbase.

## Returntype

void

## Parameters
*none*


## Description

Applying this method to a particular entry deletes it from the termbase. The corresponding entry is then removed physically from the termbase and can only be restored from a backup file (if available).

Note that only users with proper authorisation are allowed to delete termbase entries. This method does not require any parameters.

## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry with id #1 
Entry oEntry = oEntries.Item(1);

oEntry.Delete();
Debug.Write("Entry deleted successfully.");
```

