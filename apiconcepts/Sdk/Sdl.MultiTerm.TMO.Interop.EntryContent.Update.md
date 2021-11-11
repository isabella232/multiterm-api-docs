# Update method

## Name

Sdl.MultiTerm.TMO.Interop.EntryContent.Update —          Updates the content of a particular entry.



## Returntype

void



## Parameters
*none*


## Description



Applying this  method to a particular entry updates the content of this entry using the MultiTerm XML stream parameter provided.

This method is the programmatic equivalent of the Edit function in MultiTerm Workstation, which allows users to edit the content of an entry, i.e. add/delete fields or update the content of a field.
Note that before applying this method the corresponding entry needs to be [locked](Sdl.MultiTerm.TMO.Interop.Entry.LockEntry.md), to prevent other users from trying to edit the entry at the same time.

Note that in order to delete a particular field, you need to add a delete="true" attribute to the description group tag (descripGrp) to delete in the update entry content (see example below).



## Sample


```cs
//select termbase
Termbase oTb = oTbs["Termbase name"];
Entries oEntries = oTb.Entries;

//select entry
Entry oEntry = oEntries.Item(1);

//lock and edit entry
oEntry.LockEntry(Sdl.MultiTerm.TMO.Interop.MtLockingState.mtLock);

//define update content
string updateContent="<conceptGrp> ... update entry content goes here ... </conceptGrp>";

oEntry.Content=updateContent;
oEntry.Content.Update();
Debug.WriteLine("Entry content updated successfully");


Example of a field to delete:

<descripGrp delete="true"><descrip type="Subject">General</descrip></descripGrp>
```

